# NFL Blitz Pro — Modernized Roster (GameCube Memory Card Save)

A fan-made roster update for **NFL Blitz Pro** (GameCube, 2003), built by
directly editing the game's memory card save file. This replaces the
original 2003 roster with current NFL players (Madden 2027 ratings as the
data source), fills out thin position groups (e.g. fullback) with
additional real players where the base roster came up short, and adds a
handful of manually researched gap-fill players at other positions.

This is a save-file mod, not a disc mod or ROM hack. No game files from
the original disc are modified or redistributed — see **Legal /
Disclaimers** below.

---

## What's in this release

Three `.gci` memory card save files, identical in roster/stats/appearance
data but differing in how commentary audio is handled:

| File | Audio behavior |
|---|---|
| `5D-GFVE-ROSTER__3a__AUDIO1.gci` | Full audio — eligible players with a last name match is pinned to a stock-2003 commentary donor row where a name match was found. Most matches are matches of last name only. Some matches are "fuzzy" meaning you will hear last names the sound close to the correct last name. You'll hear real last names called for most players. On occasion the commentators will call out the first and last name of the stock-2003 donor |
| `5D-GFVE-ROSTER__3a__AUDIO0.gci` | All name-based commentary suppressed — every player uses the generic ("he"/"the receiver"/etc.) fallback. Use this if you'd rather never hear a wrong or mismatched name. |
| `5D-GFVE-ROSTER__3a__AUDIO2.gci` | Conservative — only exact full-name matches (first + last) are pinned to their donor's audio; everything else falls back to generic commentary. |

Pick whichever variant fits your tolerance for the occasional "wrong era"
name callout vs. generic commentary. All three have the same rosters,
stats, and appearance data — only audio behavior differs.

## Requirements

- **Dolphin Emulator or soft modded Wii or Modded Game Cube**
- **Your own legally-owned copy of NFL Blitz Pro** — this project does
  not provide the game itself (see Legal section)
- A GameCube memory card slot configured in Dolphin, with room for one
  save
- You can get the save on a memory card through a soft modded Wii, then load it on a stock Game Cube.

## Installation

1. Open Dolphin → **Tools → Memory Card Manager** (or GCMemcard Manager).
   or search for the "Card A" folder which is normally under the user folder with a path that ends like this:
   AppData\Roaming\Dolphin Emulator\GC\USA\Card A
   or on the phone connect your phone to a PC using USB and naviagate through your computer to a folder slot that looks like:
   Internal shared storage\Android\data\org.dolphinemu.dolphinemu\files\GC\USA\Card A
   
2. Import the `.gci` file of your choice (Import GCI / drag-and-drop,
   depending on your Dolphin version).
3. Boot NFL Blitz Pro and load the imported save from the roster select
   screen.
   
 4. The files can be renamed in the game. Files will not load if you rename them outside of the game.

You can load all 3 save files on to one memory card folder. .

## What's changed from the original 2003 roster

- Rosters updated using Madden 2027 ratings as the primary data source,
  converted to the Blitz stat scale.
- Positions where the stock 2003 roster (or Madden's own depth charts)
  came up short — most notably fullback — are backfilled with additional
  real players sourced from team depth charts, so every team has a full,
  playable roster with no placeholder/blank slots.
- A small number of additional real players were added by hand at other
  positions to close remaining depth-chart gaps; where a stat couldn't be
  sourced from Madden or a prior season's ratings, it was estimated from
  comparable players and is documented as such internally.
- Player names, jersey numbers, teams, and appearance (skin tone, body
  type, equipment where supported) reflect current rosters as of this
  project's data pull. **Rosters are a snapshot in time** — the NFL
  offseason moves fast, and this will not track trades, cuts, or signings
  after the date of this release.

## Known limitations

- **Commentary audio is fundamentally limited by the original 2003 voice
  recordings.** The game can only say the ~399 names that were actually
  recorded for the original release. Every current player who isn't a
  name-match to one of those original 399 will either borrow another
  player's recorded name (AUDIO1/AUDIO2) or use generic commentary
  (AUDIO0/AUDIO2 fallback). This is a hard constraint of the original
  game, not something a save-file edit can fix.
- Some appearance/equipment details are approximate — see the appearance
  data notes if you're contributing player look-ups.
- Playbooks are based on the playbooks for the original rosters so a 2027 passing team may have a running team's playbook.
  Fortunately you can select any playbook and audibles if you create a user profile and save it.
  Play books are decsribed in the game base of of the original team from 2003.
- This is a hobby project maintained on a best-effort basis, not an
  officially supported release.

## Contributing

Appearance/equipment data (skin tone, build, face, etc.) is one of the more
time-consuming parts of this project and contributions are welcome. Open
an issue or pull request if you'd like to help fill in players, or if you
spot an incorrect stat, team assignment, or name.

---

## Legal / Disclaimers

- **This release does not contain, and never has contained, any copy of
  the NFL Blitz Pro game disc, ISO, ROM, ROM image, or any extracted game
  assets (code, textures, models, audio files, etc.).** What's provided
  here is a GameCube memory card save file (`.gci`) — a small file
  containing roster data (names, stats, team assignments, appearance
  parameters) intended to be loaded by a legally-owned copy of the
  original game. You must own the game yourself to use these files; this
  project cannot and does not provide it.
- **This project is free to use, share, and redistribute.** It is not
  monetized, is not behind a paywall, and no payment, subscription, or
  "tip" is required to access any file in this release. If you paid
  someone for these specific files, you were not required to.
- **Fan project — not affiliated with or endorsed by Midway Games, WMS
  Gaming, the NFL, the NFLPA, EA Sports, or any current rights holder of
  NFL Blitz Pro or NFL Blitz.** All original game trademarks, characters,
  team names, and logos belong to their respective owners. This is an
  unofficial, non-commercial fan modification shared for personal,
  non-commercial use.
- **Player names, likenesses, and statistics** used in the roster data
  are drawn from publicly available sports statistics and ratings
  (Madden NFL ratings data) for the purpose of building an accurate,
  fan-made roster update. No official license to use current NFL player
  names, likenesses, or the NFLPA/NFL trademarks is claimed or implied by
  this project.
- **No warranty.** These files are provided "as is," without warranty of
  any kind. Use at your own risk. This project is not responsible for any
  save data corruption, memory card issues, or other problems that may
  arise from using these files. Back up your existing memory card saves
  before importing anything.
- **Takedown requests:** if you are a rights holder and have a concern
  about this project, please open an issue on this repository or contact
  the maintainer directly, and it will be addressed promptly.

---

## Credits

- Roster and appearance data compiled and maintained by the project
  owner. Appearance data entry help from Discord
  contributors — are welcome. https://discord.gg/bdMG8UUNd
- Built entirely through direct save-file editing in Dolphin Emulator;
  no disc modification, decryption circumvention, or ROM patching was
  performed.

