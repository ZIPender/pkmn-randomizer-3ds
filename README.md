# Pokemon Randomizer: beta

<img align="right" src="beta-qr.png" width="168" alt="QR code that installs the Pokemon Randomizer beta through FBI">

**2.2.0 beta 1** is a test build of the next version. The stable version,
2.1.2, is on the [main page](https://github.com/ZIPender/pkmn-randomizer-3ds).

1. On your 3DS, open **FBI** › **Remote Install** › **Scan QR Code**.
2. Point the camera at this code. It always installs the newest beta, over
   the version you have: your settings and randomized games stay.
3. Start **Pokemon Randomizer** from the HOME Menu. The first screen says
   **Version 2.2.0 beta 1**.

No camera handy? Copy `pokemon-randomizer.cia` from the
[beta release](https://github.com/ZIPender/pkmn-randomizer-3ds/releases/tag/beta-latest)
to the SD card and install it with FBI. Use the CIA rather than the `.3dsx`:
the installed app gets more memory than the Homebrew Launcher one, and only
the installed app has the HOME Menu banner.

## What's new in this beta

- **Shiny odds for Gen 3.** Ruby, Sapphire, Emerald, FireRed and LeafGreen
  now have the Shiny odds setting (Customize › Wild). Any odds from 1 in 8192
  to 1 in 256 work as typed. More often than that, the game only takes 1 in
  128, 64, 32 and so on, so a custom value goes to the closest of those. The
  most is 1 in 2: Custom 1 gives 1 in 2.
  - Trainers' Pokémon are never shiny.
  - The pictures the game always shows in normal colours stay normal: the
    starter choice, the Pokédex and the credits.
  - Spinda and Unown can still look shiny in the Pokédex.
  - A Pokémon you move to another game uses that game's normal odds there,
    so it may not be shiny anymore.
  - The English versions are checked. On another copy whose code doesn't
    match, the game keeps its normal odds and the spoiler log says so.
- **Black 2 and White 2 spoiler log.** The World Tournament teams now show
  their real levels. The game sets those levels itself, so the level setting
  never changed them.

## What to test

- A Gen 3 game at 1 in 64 or Custom 2: shiny Pokémon in the grass, while
  the starter choice, the Pokédex and the credits keep their normal colours.
  Trainer battles should start as usual.

Report what you see on the
[issues page](https://github.com/ZIPender/pkmn-randomizer-3ds/issues), with
**Options › Save a log file** turned on: your console, the game and where it
comes from, the settings code and seed, and the file
`sd:/3ds/pokemon-randomizer/logs/app.log`.

Unofficial fan project, not affiliated with Nintendo, Game Freak, Creatures
or The Pokémon Company. It contains no game data: use games you own.
