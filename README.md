# Pokemon Randomizer: beta

<img align="right" src="beta-qr.png" width="168" alt="QR code that installs the Pokemon Randomizer beta through FBI">

**2.4.0 beta 1** is a test build of the next version. The stable version,
2.3.0, is on the [main page](https://github.com/ZIPender/pkmn-randomizer-3ds).

1. On your 3DS, open **FBI** › **Remote Install** › **Scan QR Code**.
2. Point the camera at this code. It always installs the newest beta, over
   the version you have: your settings and randomized games stay.
3. Start **Pokemon Randomizer** from the HOME Menu. The first screen says
   **Version 2.4.0 beta 1**.

No camera handy? Copy `pokemon-randomizer.cia` from the
[beta release](https://github.com/ZIPender/pkmn-randomizer-3ds/releases/tag/beta-latest)
to the SD card and install it with FBI. Use the CIA rather than the `.3dsx`:
the installed app gets more memory than the Homebrew Launcher one, and only
the installed app can put games on the HOME Menu.

## New in beta 1

- **Cheats.** **Customize** has an eighth tab, **Cheats**, for every game from
  Red to Ultra Moon.
- **Instant text.** Every text box shows at once, battle text included,
  whatever text speed the game's options say. The game still waits for A at
  the end of a box and before a yes/no question.
- **Starting items.** Start a new game with 999 Rare Candies for a Nuzlocke,
  a few Master Balls or any other item the game has. Pick a group, then an
  item: A opens a number pad for how many, Left and Right take one off or add
  one. The bag holds what the game's own bag holds: the top screen shows how
  full each pocket gets. Key items, HMs, Z-Crystals and the TMs that never run
  out are one at most. In FireRed and LeafGreen the TM Case or Berry Pouch
  comes with the first TM or berry.
- Cheats are kept for each game and are not part of the settings code. Only a
  new game gets the items: a save you already have keeps its bag.
- **Yellow: Pewter Museum fixed.** A new starter no longer breaks the
  museum's first floor.
- **Omega Ruby and Alpha Sapphire: Cosplay Pikachu fixed.** Its costume no
  longer changes when gifts aren't randomized.

## What to test

- Turn on **Instant text**, randomize, and play the intro and a first battle:
  text shows at once, and boxes still wait for A.
- Pick a few starting items (Rare Candy ×999, a TM, a Poké Ball, a berry),
  randomize and start a **new game**: the items are in the bag, in the right
  pockets. Save, turn the game off and on: the bag is the same, nothing is
  given twice.
- Any game works, but these were checked less: Black and Black 2, X and Alpha
  Sapphire, and Ultra Moon.

Report what you see on the
[issues page](https://github.com/ZIPender/pkmn-randomizer-3ds/issues), with
**Options › Save a log file** turned on: your console, the game and where it
comes from, the settings code and seed, and the file
`sd:/3ds/pokemon-randomizer/logs/app.log`.

Unofficial fan project, not affiliated with Nintendo, Game Freak, Creatures
or The Pokémon Company. It contains no game data: use games you own.

The app includes curl, Mbed TLS and zlib for its update check: see
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
