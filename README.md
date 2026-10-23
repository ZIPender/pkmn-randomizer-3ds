<p align="center">
  <img src="media/hero.png" width="100%" alt="Pokemon Randomizer for Nintendo 3DS, version 2.1.0: your games, randomized on the console itself. GB, GBC, GBA, DS and 3DS games, Gen 1 to 7, 28 games. Scan the QR code with FBI to install it.">
</p>

<p align="center">
  <a href="https://github.com/ZIPender/pkmn-randomizer-3ds/releases/latest"><b>Latest release</b></a> ·
  <a href="#install">Install</a> ·
  <a href="#supported-games">Supported games</a> ·
  <a href="#how-it-works">How it works</a> ·
  <a href="https://github.com/ZIPender/pkmn-randomizer-3ds/issues">Report a bug</a>
</p>

https://github.com/user-attachments/assets/b636478c-fd76-4750-8825-a313927260f2

<p align="center">
  <img src="media/demo.gif" width="400" alt="The app's two screens: pick Pokemon Emerald, choose the Standard style, roll a seed and press Generate. The top screen fills a Poke Ball as it works, and the randomized game is ready in 7 seconds, with its spoiler log.">
</p>

Pick one of your games, choose a style, and the 3DS builds a randomized copy:
new starters, wild Pokémon, trainers, moves, items and more. It works
offline, and your original game is never modified.

## Install

<img align="right" src="install-qr.png" width="168" alt="QR code that installs Pokemon Randomizer through FBI">

1. On your 3DS, open **FBI** › **Remote Install** › **Scan QR Code**.
2. Point the camera at this code. FBI downloads and installs the latest release.
3. Start **Pokemon Randomizer** from the HOME Menu.

No camera handy? Copy `pokemon-randomizer.cia` from the
[latest release](https://github.com/ZIPender/pkmn-randomizer-3ds/releases/latest)
to the SD card and install it with FBI, or copy `pokemon-randomizer.3dsx`
to `sd:/3ds/` for the Homebrew Launcher. Version 1.x is upgraded in place.

**You need:** a 3DS, 2DS or New 3DS with
[Luma3DS](https://3ds.hacks.guide), FBI, and your own legally dumped games
(ROM files, installed 3DS games or a game card).

## Supported games

| Gen | Games | You get |
| --- | --- | --- |
| 1 | Red, Blue, Yellow | `.gb` |
| 2 | Gold, Silver, Crystal | `.gbc` |
| 3 | Ruby, Sapphire, Emerald, FireRed, LeafGreen | `.gba` |
| 4 | Diamond, Pearl, Platinum, HeartGold, SoulSilver | `.nds` |
| 5 | Black, White, Black 2, White 2 | `.nds` |
| 6 | X, Y, Omega Ruby, Alpha Sapphire | its own HOME Menu title, or a Luma3DS game patch |
| 7 | Sun, Moon, Ultra Sun, Ultra Moon | its own HOME Menu title, or a Luma3DS game patch |

At least one game of every generation was randomized and played on a New 3DS
XL. English releases are the tested ones; please report anything that goes
wrong.

## How it works

<p align="center">
  <img src="media/screens.png" width="100%" alt="Four steps on the 3DS: pick a game, choose a style, roll a seed, play your new game.">
</p>

1. Put your ROM files (`.gb .gbc .gba .nds`, decrypted `.3ds/.cci/.cxi`) in
   `sd:/roms` or folders inside it. The app also looks at the SD card's root
   and the folders right under it (not system ones like `Nintendo 3DS`,
   `luma` or `3ds`), and **Options › Folders** adds any other folder.
   Installed 3DS games and the game card are found by themselves.
2. Tap **Randomize**, pick a game and a style: **Casual**, **Standard**,
   **Chaos**, or **Custom**, where the top screen explains every option.
3. Keep or roll a seed, then **Generate**. The same game, seed and settings
   code always give the same result, so you can race friends.
4. The game is saved in its own folder, like
   `sd:/3ds/pokemon-randomizer/randomized/Emerald-Randomized-U4DM/`, with its
   spoiler log (**Options** can change where). Open it from
   **Randomized games**: **How to play** says how to start it.

**What changes:** starters, wild Pokémon, trainers, legendaries and gifts,
in-game trades, stats, types, abilities, evolutions, moves and TMs, items
on the ground, and the shiny odds of wild Pokémon (Gen 2 and Gen 4 to 7),
with a spoiler log for when you're stuck.

**Updates:** the app checks GitHub for a new version when it starts and asks
before downloading it (turn it off in **Options › Check for updates**). It
works from version 2.1.0 on; older versions update with the QR code.

**3DS games** can become their own HOME Menu title, with their own icon and
save: turn on **HOME** on the seed screen. It is a full copy of the game
(about 50 minutes on a New 3DS XL) and is still being tested on
consoles. The quick way is **Activate in Luma**, which plays it through
Luma3DS game patching with the original game's save, so back that save up
with Checkpoint first.

GB and GBA games play in mGBA or any emulator; DS games in TWiLight Menu++
or on a flashcart.

<details>
<summary><b>Troubleshooting</b></summary>

- **A game is missing:** check that the file is in `sd:/roms` (or at most two
  folders inside it), or add its folder in **Options › Folders**, and that it
  is a clean, decrypted dump, then press X on the game list.
- **FBI's QR install stalls at 0%:** your 3DS can't reach GitHub over HTTPS.
  Use the manual install.
- **"Something went wrong":** the dump looks modified or damaged. Your game
  was not changed; **View log** shows the details.

Report bugs on the [issues page](https://github.com/ZIPender/pkmn-randomizer-3ds/issues)
with the game and region, the seed and settings code, and what you saw.
</details>

## Disclaimer

Unofficial fan project, not affiliated with Nintendo, Game Freak, Creatures
or The Pokémon Company. It contains no game data: use games you own.

The app includes curl, Mbed TLS and zlib for its update check: see
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
