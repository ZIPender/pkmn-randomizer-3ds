# Pokemon Randomizer: beta

<img align="right" src="beta-qr.png" width="168" alt="QR code that installs the Pokemon Randomizer beta through FBI">

**2.4.1 beta 1** is a test build of the next version. The stable version,
2.4.0, is on the [main page](https://github.com/ZIPender/pkmn-randomizer-3ds).

1. On your 3DS, open **FBI** › **Remote Install** › **Scan QR Code**.
2. Point the camera at this code. It always installs the newest beta, over
   the version you have: your settings and randomized games stay.
3. Start **Pokemon Randomizer** from the HOME Menu. The first screen says
   **Version 2.4.1 beta 1**.

No camera handy? Copy `pokemon-randomizer.cia` from the
[beta release](https://github.com/ZIPender/pkmn-randomizer-3ds/releases/tag/beta-latest)
to the SD card and install it with FBI. Use the CIA rather than the `.3dsx`:
the installed app gets more memory than the Homebrew Launcher one, and only
the installed app can put games on the HOME Menu.

## New in beta 1

- **Omega Ruby and Alpha Sapphire: DexNav fixed.** Opening the DexNav froze
  the game in areas with more wild Pokémon than its list can hold (Chaos, or
  Custom with random wild Pokémon). Those areas now keep few enough. A game
  made with 2.4.0 still freezes there: make it again from its page, with the
  same seed and settings code. Only the crowded areas change.
- **Choose a style: X and Y.** On Casual, Standard or Chaos, **Y** lists
  everything the style changes: the top screen only has room for the first
  few. **X** opens Custom with that style's settings, ready to change. If you
  already have Custom settings of your own, it asks before replacing them.
- **Instant text comes with Standard and Chaos.** Casual keeps the game's own
  text speed, and Custom keeps what you chose.
- **The story names your new starters.** Lines that still named the original
  starters now follow the new ones: in Sun, Moon, Ultra Sun and Ultra Moon,
  the introductions, the choice scene, what Kukui and Hau say about your
  starter and Hau's, and Hau's first defeat in the Ultra games; the Mechadoll
  quiz in Omega Ruby and Alpha Sapphire; the lesson on types in Omega Ruby,
  Alpha Sapphire, Ruby, Sapphire and Emerald; your rival's and your friend's
  starters in Diamond, Pearl and Platinum; in Black, White, Black 2 and
  White 2, the lines that name the starters or the type they are weak to, and
  the item given for your starter's type. The lesson on types is English
  only, the lines of Sun, Moon, Ultra Sun and Ultra Moon in Chinese keep the
  original names, and the Pokémon you see in their choice scene are still the
  original three. With Trainer teams on Unchanged, your rival's starter now
  follows the new starters too, so the battle shows the Pokémon the story
  names.
- **Diamond, Pearl, Platinum:** Professor Rowan no longer tells you your new
  starter has evolved, and the three people who give a mask chosen by your
  starter (Jubilife TV, Pastoria City, the Veilstone Department Store)
  recognise the new starters.
- **Black 2 and White 2: the Habitat List** shows each area's new wild
  Pokémon, and its stamps ask for them. It has room for 30 species an area
  and 20 a page: in a crowded area (Chaos), the rarest ones live there
  without being listed.
- **Every family catchable** no longer counts on places you can't reach:
  Altering Cave's Mystery Gift sets (Emerald, FireRed, LeafGreen), Mirage
  Island (Ruby, Sapphire, Emerald) and the Pokémon a GBA game in the DS's
  second slot brings (Diamond, Pearl, Platinum).
- **HeartGold and SoulSilver:** the mystery egg from Mr. Pokémon is always
  the Pokémon the spoiler log names.

## What to test

- Omega Ruby or Alpha Sapphire on **Chaos**: once you have the DexNav, open
  it on every route, cave and water route you reach.
- **Choose a style**: press **Y** on each style and read the list. Press
  **X** on Standard, change an option and randomize: your Custom settings
  change, Standard itself stays the same.
- **Starter names**: start a new game with random starters and play to
  your first rival battle (in Sun, Moon, Ultra Sun or Ultra Moon, to the
  festival in Iki Town). Every line that names a starter should name one of
  the three you were offered.
- **Black 2 or White 2**: open the Pokédex's Habitat List on the routes you
  have been to. Its Pokémon should be the spoiler log's, and a page's stamp
  should come once you have seen every Pokémon on it.
- **Every family catchable** on Emerald, FireRed, LeafGreen, Diamond, Pearl
  or Platinum: the spoiler log's Wild section says how many families are in
  the wild, and names any left out.

Report what you see on the
[issues page](https://github.com/ZIPender/pkmn-randomizer-3ds/issues), with
**Options › Save a log file** turned on: your console, the game and where it
comes from, the settings code and seed, and the file
`sd:/3ds/pokemon-randomizer/logs/app.log`.

Unofficial fan project, not affiliated with Nintendo, Game Freak, Creatures
or The Pokémon Company. It contains no game data: use games you own.

The app includes curl, Mbed TLS and zlib for its update check: see
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
