# Pokemon Randomizer: beta

<img align="right" src="beta-qr.png" width="168" alt="QR code that installs the Pokemon Randomizer beta through FBI">

**2.1.1 beta 2** is a test build of the next version. The stable version,
2.1.0, is on the [main page](https://github.com/ZIPender/pkmn-randomizer-3ds).

1. On your 3DS, open **FBI** › **Remote Install** › **Scan QR Code**.
2. Point the camera at this code. It always installs the newest beta, over
   the version you have: your settings and randomized games stay.
3. Start **Pokemon Randomizer** from the HOME Menu. The first screen says
   **Version 2.1.1 beta 2**.

No camera handy? Copy `pokemon-randomizer.cia` from the
[beta release](https://github.com/ZIPender/pkmn-randomizer-3ds/releases/tag/beta-latest)
to the SD card and install it with FBI. Use the CIA rather than the `.3dsx`:
the installed app gets more memory than the Homebrew Launcher one.

## What's new in this beta

- **Custom shiny odds.** On the Wild tab, **Shiny odds › Custom** opens the
  number keypad: type N for 1 in N. 1 makes every wild Pokémon shiny, 36
  means 1 in 36. Some games can only get close, and the app and the spoiler
  log say what each game really gets:
  - Gold, Silver and Crystal only do 1 in 2, 4, 8, 16... (36 gives 1 in 32);
  - Diamond to White 2 stop at 255 in 256: those games would freeze if no
    wild Pokémon could be normal.
- **Shiny odds** is now right under **Similar strength** on the Wild tab.
- **Excluded folders**, asked for in
  [#1](https://github.com/ZIPender/pkmn-randomizer-3ds/issues/1):
  **Options › Scan folders › Exclude**. An excluded folder and everything
  inside it are never searched, so games you don't want to randomize (fan-made
  games, for example) stay out of the list.
- **What's new** (new in beta 2). After an update, the app shows once what
  the new version brings, and **Options › What's new** lists every version's
  changes.

Settings codes from 2.1.0 give the same games. A code with custom odds is 5
characters longer and needs this beta or newer.

## What to test

- Custom odds in your games, above all **Platinum, White, Black, Diamond,
  Pearl, HeartGold and SoulSilver at 1**: play a few routes, get an egg or a
  gift Pokémon, and tell us if anything freezes.
- Excluded folders with your own folders.
- Installing over an older version (2.1.0 or beta 1): the **What's new** card
  shows once, then never again for this version. A first install shows
  nothing.
- When 2.1.1 comes out, the app offers it by itself.

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

Unofficial fan project, not affiliated with Nintendo, Game Freak, Creatures
or The Pokémon Company. It contains no game data: use games you own.

The app includes curl, Mbed TLS and zlib for its update check: see
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
