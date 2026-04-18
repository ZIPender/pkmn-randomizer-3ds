# Pokémon Randomizer for 3DS

On-device Pokémon ROM randomizer. Drop your ROM dumps on the SD card, pick a
seed, and the 3DS writes randomized copies you can play in any compatible
emulator or flashcart.

No PC. No phone. Just the handheld.

**Supported games** (requires your own legally-dumped ROMs):

| Gen | Games |
| --- | --- |
| 1 | Red, Blue, Yellow |
| 2 | Gold, Silver, Crystal |
| 3 | Ruby, Sapphire, Emerald, FireRed, LeafGreen |
| 4 | Diamond, Pearl, Platinum |
| 5 | Black, White, Black 2, White 2 |

**What it randomizes**: starters (with sprite + name updates where possible),
wild encounters, trainer teams, evolutions. Settings like type-theme
preservation, BST balancing, and legendary allowance are configurable in-app.

## Requirements

- Nintendo 3DS / 2DS / New3DS with **custom firmware** (Luma3DS).
  If you haven't modded yet: follow [3ds.hacks.guide](https://3ds.hacks.guide).
- **FBI** (to install the CIA) or **Homebrew Launcher** (to run the .3dsx).
- Your own ROM dumps placed on the SD card (see below).

## Install — scan the QR code

In **FBI → Remote Install → Scan QR Code**, point the 3DS camera at:

![Install QR](install-qr.png)

FBI will download and install `pokemon-randomizer.cia` directly. The app
appears on the HOME menu.

### Alternative: manual install

- **CIA (recommended)**: copy `pokemon-randomizer.cia` to your SD card,
  open FBI → *SD → pokemon-randomizer.cia → Install and delete CIA*.
- **3DSX (Homebrew Launcher)**: copy `pokemon-randomizer.3dsx` to
  `sdmc:/3ds/pokemon-randomizer/` and launch from the Homebrew Launcher.

## Put your ROMs on the SD card

The app auto-detects ROMs in any of these folders (case-insensitive):

```
sdmc:/roms/
sdmc:/Roms/
sdmc:/ROMS/
sdmc:/3ds/roms/
```

Supported extensions: `.gb`, `.gbc`, `.gba`, `.nds`.

## Use it

1. Launch **Pokemon Randomizer** from the HOME menu.
2. **Detected Games** → press **A** on a title to select it.
3. **Seed** → pick a number (Y = random from system tick).
4. **Settings** → tweak presets, legendaries, type themes, BST balance, etc.
5. **Generate** → press **A** on *Generate patch*. Wait for *Finished*.
6. Randomized ROM lands at:

   ```
   sdmc:/3ds/pokemon-randomizer/output/<game>/<rom-name>/<rom-name>-randomized.<ext>
   ```

   Alongside it: `starters.txt` (what got rolled) and `randomizer.manifest`
   (seed + settings, so you can reproduce a run).

7. Copy the randomized ROM off the SD card, or load it on a flashcart /
   emulator directly from there.

## Troubleshooting

- **"No detected games"** — make sure ROMs are in one of the folders above
  and the extensions are correct.
- **"Could not write randomized output ROM"** — SD card out of space or
  write-protected.
- **"LZ decompress failed for species N"** (Gen 5 only) — non-fatal, the
  app keeps the original sprite for that species and continues.
- **FBI QR install stalls at 0%** — your 3DS can't reach GitHub over HTTPS;
  try the manual CIA install instead.

## Reporting bugs

Open an issue at
<https://github.com/ZIPender/pkmn-randomizer-3ds/issues> with:
- game + region
- seed
- settings you used
- what you saw vs. what you expected

## Legal

Ship your own ROM dumps of games you own. This tool does **not** distribute
copyrighted content. Randomized output stays on your SD card.
