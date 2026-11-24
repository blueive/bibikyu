# bibikyu

bibikyu splits one `.ass` subtitle file into several files, one per translator, so the work can be shared out.

Windows 10/11 (64-bit). Nothing to install, and no internet connection needed.

## How to use it

1. Click **Browse…** and pick your `.ass` file. bibikyu shows how many dialogue lines it has.
2. Type the episode name.
3. Set the number of translators and type their names. The lines are split evenly in order (8 lines for 5 people gives 2, 2, 2, 1, 1). You can change any number yourself afterwards.
4. Tick **Add credit line** if you want an empty line from 0:00:00 to 0:00:05 at the end of each file. Otherwise leave it unticked.
5. Choose the output folder and click **Generate files**.

You get one file per translator, named like this:

```
Episode - (1) Person_Name1.ass
Episode - (2) Person_Name2.ass
...
```

Each file keeps everything from the original (styles, script info, timings, tags) and holds only that translator's lines. Your original file is never changed.

If a file with the same name already exists, bibikyu asks before replacing it.

## Good to know

- Only `Dialogue` lines are counted. Comment lines go with the line just after them, so nothing is duplicated.
- Line counts must add up exactly to the file's total. Until they do, the Generate button stays off and a message tells you what's wrong.
- The files open normally in Aegisub.

## "Windows protected your PC"

bibikyu isn't signed, so Windows may show this the first time you open it. Click **More info**, then **Run anyway**. Some antivirus programs may flag it for the same reason.

---

Made by bibi. See `LICENSE.txt` for the terms of use.
