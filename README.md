# Pokemon Randomizer: beta

<img align="right" src="beta-qr.png" width="168" alt="QR code that installs the Pokemon Randomizer beta through FBI">

**2.2.0 beta 2** is a test build of the next version. The stable version,
2.1.2, is on the [main page](https://github.com/ZIPender/pkmn-randomizer-3ds).

1. On your 3DS, open **FBI** › **Remote Install** › **Scan QR Code**.
2. Point the camera at this code. It always installs the newest beta, over
   the version you have: your settings and randomized games stay.
3. Start **Pokemon Randomizer** from the HOME Menu. The first screen says
   **Version 2.2.0 beta 2**.

No camera handy? Copy `pokemon-randomizer.cia` from the
[beta release](https://github.com/ZIPender/pkmn-randomizer-3ds/releases/tag/beta-latest)
to the SD card and install it with FBI. Use the CIA rather than the `.3dsx`:
the installed app gets more memory than the Homebrew Launcher one, and only
the installed app can put games on the HOME Menu.

## What's new in this beta

- **Every generation on the HOME Menu.** Like 3DS games already could, a
  randomized Gen 1 to 5 game now gets its own HOME Menu icon: turn on
  **HOME** on the seed screen (X), or pick **Add to HOME Menu** on the
  game's page. It needs the CIA build, started from the HOME Menu, and
  Luma3DS.
  - **GBA games** (Ruby, Sapphire, Emerald, FireRed, LeafGreen) become a
    Virtual Console title that runs in the 3DS's own GBA mode, with its own
    save (about 17 MB, a minute to install). Quit with **HOME**, then **A**:
    the save is written only then. Removing the title backs its save up
    first.
  - **DS games** (Gen 4 and 5) get a small icon that starts them with
    nds-bootstrap. It needs the **"YANBF Forwarder Pack"**: install it with
    **Universal-Updater**.
  - **GB and GBC games** (Gen 1 and 2) get a small icon that starts them in
    mGBA. It needs mGBA's development build: in **Universal-Updater**, pick
    **mGBA** and install **"[git] mgba.cia"**. The stable mGBA can't open a
    game from another icon.
  - For DS, GB and GBC games, the game stays in its folder and its save stays
    next to it, as when you play it from TWiLight Menu++ or mGBA. The app
    tells you what to install when something is missing.
- **Every family catchable** (Customize › Wild, off by default). The first
  form of every evolution family, Pokémon that don't evolve included, gets a
  wild spot before the rest is randomized. Everything else is then caught in
  the wild or one evolution away, random evolutions included, so the whole
  Pokédex can be filled in one game.
  - It works with Random and Area 1:1. Global 1:1 swaps species one for one,
    so it only fits as many families as the game has wild species.
  - Legendaries and mythicals are placed too when **Legendaries in pools**
    is on. Trade evolutions need **No trade evolutions** (on by default).
  - It can't be on with **Similar strength**: turn that off first.
  - The spoiler log's Wild section says how many families made it.
- From beta 1: **shiny odds for Gen 3** (Ruby to LeafGreen, 1 in 8192 up to
  1 in 2), and the Black 2 and White 2 World Tournament levels in the
  spoiler log.

## What to test

- A **DS game** on the HOME Menu, with the YANBF Forwarder Pack installed:
  add it, start it from its icon, save, and start it again.
- A **GB or GBC game** on the HOME Menu, with "[git] mgba.cia" installed:
  the same.
- Without those tools installed, the app should say which one to get.
- A **GBA game** on the HOME Menu: play, save (HOME, then A), start again.
- **Every family catchable**: Standard style with Similar strength off, or
  Chaos, then this option. The spoiler log should say every family is in
  the wild.

Report what you see on the
[issues page](https://github.com/ZIPender/pkmn-randomizer-3ds/issues), with
**Options › Save a log file** turned on: your console, the game and where it
comes from, the settings code and seed, and the file
`sd:/3ds/pokemon-randomizer/logs/app.log`.

Unofficial fan project, not affiliated with Nintendo, Game Freak, Creatures
or The Pokémon Company. It contains no game data: use games you own.
