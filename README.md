# Pokémon Randomizer for 3DS

A Pokémon randomizer that runs on the 3DS itself. Pick one of your games,
choose a style, and the console builds a randomized copy: new starters,
wild Pokémon, trainers, moves, items and more. Everything stays offline, and
your original game is never modified.

**Version 2.0** supports every main-series generation from Red to Ultra Moon,
with a touch-friendly interface on both screens.

| Gen | Games | Randomized game |
| --- | --- | --- |
| 1 | Red, Blue, Yellow | `.gb` |
| 2 | Gold, Silver, Crystal | `.gbc` |
| 3 | Ruby, Sapphire, Emerald, FireRed, LeafGreen | `.gba` |
| 4 | Diamond, Pearl, Platinum, HeartGold, SoulSilver | `.nds` |
| 5 | Black, White, Black 2, White 2 | `.nds` |
| 6 | X, Y, Omega Ruby, Alpha Sapphire | Luma3DS game patch |
| 7 | Sun, Moon, Ultra Sun, Ultra Moon | Luma3DS game patch |

2.0 is new: Gen 1–5 were tested on real games; Gen 6 and 7 have not yet run
on a real console. Please report what you find.

## Requirements

- A 3DS, 2DS or New 3DS with **Luma3DS** custom firmware
  ([3ds.hacks.guide](https://3ds.hacks.guide)).
- **FBI** to install the CIA, or the Homebrew Launcher for the `.3dsx`.
- Your own legally dumped games: ROM files, installed 3DS games or a game card.

## Install: scan the QR code

In **FBI → Remote Install → Scan QR Code**, point the camera at:

![Install QR](install-qr.png)

FBI downloads the latest release and installs it. If 1.x is installed, it
is upgraded in place.

**Manual install:** copy `pokemon-randomizer.cia` to the SD card and install
it with FBI, or copy `pokemon-randomizer.3dsx` to `sd:/3ds/` and start it from
the Homebrew Launcher. The CIA can also read installed games and game cards.

## Use it

1. Put ROM files (`.gb .gbc .gba .nds`, decrypted `.3ds/.cxi`) in `sd:/roms`.
   Installed 3DS games and the inserted game card are found automatically.
2. Start **Pokemon Randomizer**, tap **Randomize** and pick a game.
3. Choose a style: Casual, Standard, Chaos, or Custom with every option
   explained on the top screen.
4. Keep or type a seed, then **Generate**. The same game, seed and settings
   code always give the same result, so you can race friends.
5. Open your randomized game from **My gifts**: **How to play** explains how
   to start it, and 3DS games are switched on with **Activate in Luma**.

GB/GBA games play in mGBA or any emulator, DS games in TWiLight Menu++ or a
flashcart. Back up your 3DS save (Checkpoint) before playing a randomized 3DS
game, since it uses the same save as the original.

## Troubleshooting

- **A game is missing:** check that the file is in `sd:/roms` (up to three
  folders deep) and is a clean, decrypted dump, then press X on the game list.
- **FBI QR install stalls at 0%:** your 3DS can't reach GitHub over HTTPS;
  use the manual install.
- **"The gift couldn't be made":** the dump looks modified or damaged. Your
  game was not changed; **View log** shows details.

Report bugs at <https://github.com/ZIPender/pkmn-randomizer-3ds/issues> with
the game and region, the seed and settings code, and what you saw.

## Disclaimer

Unofficial fan project, not affiliated with Nintendo, Game Freak, Creatures
or The Pokémon Company. It contains no game data: use games you own.
