# Pokemon Randomizer: beta

<img align="right" src="beta-qr.png" width="168" alt="QR code that installs the Pokemon Randomizer beta through FBI">

**2.4.2 beta 1** is a test build of the next version. The stable version,
2.4.1, is on the [main page](https://github.com/ZIPender/pkmn-randomizer-3ds).

1. On your 3DS, open **FBI** › **Remote Install** › **Scan QR Code**.
2. Point the camera at this code. It always installs the newest beta, over
   the version you have: your settings and randomized games stay.
3. Start **Pokemon Randomizer** from the HOME Menu. The first screen says
   **Version 2.4.2 beta 1**.

No camera handy? Copy `pokemon-randomizer.cia` from the
[beta release](https://github.com/ZIPender/pkmn-randomizer-3ds/releases/tag/beta-latest)
to the SD card and install it with FBI. Use the CIA rather than the `.3dsx`:
the installed app gets more memory than the Homebrew Launcher one, and only
the installed app can put games on the HOME Menu.

## New in beta 1

- **X and Y no longer freeze at the Tower of Mastery.** Korrina gives you a
  Lucario holding its Lucarionite, and her battle there makes it Mega
  Evolve. With *Legendaries & gifts* randomized, the gift became another
  Pokémon still holding the Lucarionite, which can't Mega Evolve, and the
  game hung there. Korrina's Lucario now always stays Lucario, and the
  spoiler log marks it "kept: the story needs it". Every other gift and
  one-time encounter is randomized as before, in every game.
- A game made with an older version still freezes there: make it again from
  its page, with the same seed and settings code. Only Korrina's Lucario
  changes, everything else stays the same.
- Every other gift and one-time encounter of the 28 games was checked for the
  same kind of trap: one the story needs as it is. The other cases (the X
  and Y box legendary, Black and White's Reshiram and Zekrom, Omega Ruby and
  Alpha Sapphire's Rayquaza) were already handled, so they stay random.

## What to test

- **X or Y** with *Legendaries & gifts* on Random (Chaos) or Similar
  (Standard): beat Korrina in Shalour City, go to the Tower of Mastery,
  take her Lucario and play through her battle there, Mega Evolution
  included.
- If any other story event in any game stops you because of a randomized
  Pokémon, report it.

Report what you see on the
[issues page](https://github.com/ZIPender/pkmn-randomizer-3ds/issues), with
**Options › Save a log file** turned on: your console, the game and where it
comes from, the settings code and seed, and the file
`sd:/3ds/pokemon-randomizer/logs/app.log`.

Unofficial fan project, not affiliated with Nintendo, Game Freak, Creatures
or The Pokémon Company. It contains no game data: use games you own.

The app includes curl, Mbed TLS and zlib for its update check: see
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
