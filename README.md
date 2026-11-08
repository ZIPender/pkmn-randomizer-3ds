# Pokemon Randomizer: beta

<img align="right" src="beta-qr.png" width="168" alt="QR code that installs the Pokemon Randomizer beta through FBI">

**2.4.4 beta 1** is a test build of the next version. The stable version,
2.4.3, is on the [main page](https://github.com/ZIPender/pkmn-randomizer-3ds).

1. On your 3DS, open **FBI** › **Remote Install** › **Scan QR Code**.
2. Point the camera at this code. It always installs the newest beta, over
   the version you have: your settings and randomized games stay.
3. Start **Pokemon Randomizer** from the HOME Menu. The first screen says
   **Version 2.4.4 beta 1**.

No camera handy? Copy `pokemon-randomizer.cia` from the
[beta release](https://github.com/ZIPender/pkmn-randomizer-3ds/releases/tag/beta-latest)
to the SD card and install it with FBI. Use the CIA rather than the `.3dsx`:
the installed app gets more memory than the Homebrew Launcher one, and only
the installed app can put games on the HOME Menu.

## New in beta 1

- **Fossils are always randomized**, in every style and every game with
  fossils (all but Gold, Silver and Crystal). Before, they only changed with
  *Legendaries & gifts* on *Swap similar* or *Random*: with Casual, an Armor
  Fossil still gave Shieldon. Now, even with *Legendaries & gifts* on
  *Unchanged*, each fossil revives into another Pokémon of similar strength
  (a legendary only with *Legendaries in pools*). The spoiler log lists them
  under "Fossils".
- **The fossil lab names the Pokémon you get** in X, Y, Omega Ruby, Alpha
  Sapphire, Sun, Moon, Ultra Sun and Ultra Moon. With fossils randomized, the
  scientist still said the original name ("This is Shieldon!") while giving
  another Pokémon.
- A game made with an older version keeps its old fossils: make it again from
  its page, with the same seed and settings code. With Standard or Chaos,
  only the lab's lines change; with Casual, the fossils change too. Nothing
  else changes.

Thanks to the player who reported the Armor Fossil in Omega Ruby
([issue #6](https://github.com/ZIPender/pkmn-randomizer-3ds/issues/6)).

## What to test

- **Any game with fossils**, made with **Casual**: revive a fossil. You
  should get the Pokémon the spoiler log's "Fossils" section names, not the
  usual one.
- **Omega Ruby or Alpha Sapphire** in particular: revive a fossil at the
  Devon Corporation in Rustboro City and check that the scientist names the
  Pokémon you receive.
- X, Y, Sun, Moon, Ultra Sun and Ultra Moon: the same check at their fossil
  labs.

Report what you see on the
[issues page](https://github.com/ZIPender/pkmn-randomizer-3ds/issues), with
**Options › Save a log file** turned on: your console, the game and where it
comes from, the settings code and seed, and the file
`sd:/3ds/pokemon-randomizer/logs/app.log`.

Unofficial fan project, not affiliated with Nintendo, Game Freak, Creatures
or The Pokémon Company. It contains no game data: use games you own.

The app includes curl, Mbed TLS and zlib for its update check: see
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
