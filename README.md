# Pokemon Randomizer: beta

<img align="right" src="beta-qr.png" width="168" alt="QR code that installs the Pokemon Randomizer beta through FBI">

**2.1 beta 2** is a test build of the next version. The stable version, 2.0,
is on the [main page](https://github.com/ZIPender/pkmn-randomizer-3ds).

Beta 1 closed at start on a New 3DS with "An exception occurred". Beta 2
fixes that: scan the code again to update.

1. On your 3DS, open **FBI** › **Remote Install** › **Scan QR Code**.
2. Point the camera at this code. It always installs the newest beta, over
   the version you have: your settings and randomized games stay.
3. Start **Pokemon Randomizer** from the HOME Menu. The first screen says
   **Version 2.1 beta 2**.

No camera handy? Copy `pokemon-randomizer.cia` from the
[beta release](https://github.com/ZIPender/pkmn-randomizer-3ds/releases/tag/beta-latest)
to the SD card and install it with FBI. Use the CIA rather than the `.3dsx`:
the installed app gets more memory than the Homebrew Launcher one.

## What this beta fixes

- **"Out of memory" on an Old 3DS, Old 3DS XL or 2DS** with DS and 3DS games.
  These consoles give the app 64 MB instead of 124 MB on a New 3DS. The app
  now needs much less (X and Y went from 55 MB to 12 MB, Platinum from 31 MB
  to 19 MB) and keeps more of that memory for randomizing. GB and GBA games
  were never affected.
- **"Missing game file a/0/1/1"** with Ultra Sun and Ultra Moon. When the
  app could not open the installed game's own files, it went on with the
  update's files alone. It now stops and shows the real error.
- If the console still runs out of memory, the message says so, and the log
  records memory use at each step.

The randomized games are the same as with 2.0: the same game, seed and
settings code give the same result.

## What to test

- Randomize a DS or 3DS game on an **Old 3DS, Old 3DS XL, 2DS or New 2DS XL**.
- Ultra Sun or Ultra Moon installed with their update.
- **Platinum:** open the Pokédex in a randomized game. A crash was reported
  there and has not been reproduced yet.

## Report what you see

Turn on **Options › Save a log file** before you randomize, then open an
[issue](https://github.com/ZIPender/pkmn-randomizer-3ds/issues) (or reply where
you got this link) with:

- your console (Old 3DS, 2DS, New 3DS XL...) and whether you started the app
  from the HOME Menu or the Homebrew Launcher;
- the game, its region, and where it comes from (ROM file, installed game,
  game card);
- the style or settings code, and the seed;
- what happened, and the file `sd:/3ds/pokemon-randomizer/logs/app.log`.

It works fine? Say so too, with your console model.

## Back to the stable version

Scan the QR code on the [main page](https://github.com/ZIPender/pkmn-randomizer-3ds)
with FBI. It installs 2.0 over the beta, and your randomized games stay.

Unofficial fan project, not affiliated with Nintendo, Game Freak, Creatures
or The Pokémon Company. It contains no game data: use games you own.
