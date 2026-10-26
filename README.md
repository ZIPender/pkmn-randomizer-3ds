# Pokemon Randomizer: beta

<img align="right" src="beta-qr.png" width="168" alt="QR code that installs the Pokemon Randomizer beta through FBI">

**2.2.2 beta 1** is a test build of the next version. The stable version,
2.2.1, is on the [main page](https://github.com/ZIPender/pkmn-randomizer-3ds).

1. On your 3DS, open **FBI** › **Remote Install** › **Scan QR Code**.
2. Point the camera at this code. It always installs the newest beta, over
   the version you have: your settings and randomized games stay.
3. Start **Pokemon Randomizer** from the HOME Menu. The first screen says
   **Version 2.2.2 beta 1**.

No camera handy? Copy `pokemon-randomizer.cia` from the
[beta release](https://github.com/ZIPender/pkmn-randomizer-3ds/releases/tag/beta-latest)
to the SD card and install it with FBI. Use the CIA rather than the `.3dsx`:
the installed app gets more memory than the Homebrew Launcher one, and only
the installed app can put games on the HOME Menu.

## New in beta 1

- **Name your games.** Five Emeralds in the list? In **Randomize › Choose a
  game**, press **Y** or tap the pencil at the end of a row, and type a name
  ("Moemon", "Emerald Kaizo"). The list shows your name, with the game and
  where it comes from under it. A named game's pencil offers **Rename** and
  **Remove name**.
- **Names stay.** They are saved on the SD card
  (`sd:/3ds/pokemon-randomizer/game-names.ini`), so they are still there
  after you turn the console off. Move or rename the ROM file and the name
  follows it at the next search: the app recognises the file by its size and
  a quick fingerprint of its contents.
- **Randomized games take the name.** A game you named starts as "Moemon
  Randomized" instead of "Emerald Randomized".

## What to test

- Name a few ROM hacks of the same game, restart the app: the names are
  still there.
- Move or rename a named ROM file on the SD card, then **Search again** (X):
  the name follows it.
- Rename a game, then remove its name.

Report what you see on the
[issues page](https://github.com/ZIPender/pkmn-randomizer-3ds/issues), with
**Options › Save a log file** turned on: your console, the game and where it
comes from, the settings code and seed, and the file
`sd:/3ds/pokemon-randomizer/logs/app.log`.

Unofficial fan project, not affiliated with Nintendo, Game Freak, Creatures
or The Pokémon Company. It contains no game data: use games you own.
