# Pokemon Randomizer: beta

<img align="right" src="beta-qr.png" width="168" alt="QR code that installs the Pokemon Randomizer beta through FBI">

**2.2.0 beta 4** is a test build of the next version. The stable version,
2.1.2, is on the [main page](https://github.com/ZIPender/pkmn-randomizer-3ds).

1. On your 3DS, open **FBI** › **Remote Install** › **Scan QR Code**.
2. Point the camera at this code. It always installs the newest beta, over
   the version you have: your settings and randomized games stay.
3. Start **Pokemon Randomizer** from the HOME Menu. The first screen says
   **Version 2.2.0 beta 4**.

No camera handy? Copy `pokemon-randomizer.cia` from the
[beta release](https://github.com/ZIPender/pkmn-randomizer-3ds/releases/tag/beta-latest)
to the SD card and install it with FBI. Use the CIA rather than the `.3dsx`:
the installed app gets more memory than the Homebrew Launcher one, and only
the installed app can put games on the HOME Menu.

## New in beta 4

- **The real time.** "Made in" on the result screen now counts the whole
  wait, the HOME Menu step included (an Emerald said 19 s for about 3
  minutes).
- **No more "stuck at 50%".** When a game is added to the HOME Menu, the
  system takes a while to start the install. The bar now says step 2,
  "installing", during that wait instead of sitting on step 1.

## New in beta 3

- **Your game's name on the HOME Menu.** A GB, GBC, GBA or DS game you add
  to the HOME Menu now shows the name you gave it, with the game under it
  ("Pokemon White, randomized").
- **Its own animated banner.** The app's banner (the ball hops and opens,
  Pokémon glitch through) with your name as the title, scrambled in the
  glitches, and the game under the ball. Short names are big, long ones
  wrap onto more lines: any name from 1 to 40 characters fits.
- **Icons.** DS games use their own icon, read from your game. GB, GBC and
  GBA games, which have none, get a new icon drawn in the same style.
- Titles you added with beta 2 keep their old name and banner: remove them
  from the HOME Menu (on the game's page) and add them again.

## Also in 2.2.0

- **Every generation on the HOME Menu.** Like 3DS games already could, a
  randomized Gen 1 to 5 game gets its own HOME Menu icon: turn on **HOME**
  on the seed screen (X), or pick **Add to HOME Menu** on the game's page.
  It needs the CIA build, started from the HOME Menu, and Luma3DS.
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
- **Shiny odds for Gen 3** (Ruby to LeafGreen, 1 in 8192 up to 1 in 2), and
  the Black 2 and White 2 World Tournament teams show their real levels in
  the spoiler log.

## What to test

- Add a game to the HOME Menu with a custom name: the balloon shows your
  name, and the banner shows it too, without spilling out. Try a short name
  and a long one.
- A **DS game** on the HOME Menu, with the YANBF Forwarder Pack installed:
  its own icon, start it from there, save, and start it again.
- A **GB or GBC game** on the HOME Menu, with "[git] mgba.cia" installed:
  the same.
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
