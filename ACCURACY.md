# Accuracy method

Every shmupfan core is checked against evidence. Every difference from MAME is
documented with its cause. We do not decap chips or measure boards ourselves:
we use published die-level models, chip and board documentation, PCB footage,
measurements shared by board owners, and MAME, ranked as below.

## Evidence, highest first

| Rank | Source | Examples |
|---|---|---|
| 1 | Real-board measurements (shared by board owners) | Scope, logic analyser, frequency counter, direct audio capture |
| 2 | Die-level models of decapped chips | fx68k, Nuked-OPM/OPN/OPL, IKA cores |
| 3 | Manufacturer documents | Schematics, parts lists, service manuals, datasheets (second reader for any reading that changes the design) |
| 4 | Real boards observed | Direct PCB captures (60 fps preferred), 1CC runs, repair logs |
| 5 | MAME | Frame-by-frame reference; its TODOs mark its guesses |
| 6 | Other cores and emulators | Reference only |

Higher wins on conflict. With nothing above MAME, the core follows MAME and an
open research item names the evidence needed.

## Verification

- ROMs and memory images byte-identical to MAME's.
- Video replayed against MAME on every captured frame (attract, gameplay, flip, all sets) plus synthetic stress scenes.
- Full system booted from power-on in simulation; every video, sound and I/O write compared with MAME.
- Sound command streams, status reads and level compared with MAME.
- MiSTer build simulated through ROM loading and SDRAM.
- Played on a MiSTer before release.

## Published per core

Findings with numbers, every MAME difference with cause and evidence, open
research items, and the origin and changes of every borrowed component.

## Upstream

Each core pins the MAME version it was verified against and is re-checked when
that driver changes. Where evidence shows MAME is wrong, we file a MAME bug
report with the evidence. Changes to borrowed components are documented in each
core's provenance file for their authors.

## Standard features (all cores from the October 2026 updates)

HDMI integer scaling, 216-line crop where the game is 224 lines, rotation;
native timing on CRT, with the game's Flip Screen DIP for monitors mounted the
other way; volume; MAME keyboard defaults; all known DIP switches; pause.

## Evidence wanted

Open an issue in the core's repository if you can provide any of these:

- Refresh rate or line count measured on any of our boards (Final Star Force is the least certain).
- 60 fps captures of scene changes in 1945k III or Solite Spirits, and of text appearing in Final Star Force.
- Cocktail mode on Last Mission or Gondomania (do sprites flip with the screen?).
- Attract-mode audio of Blue Hawk or Flying Tiger.
- Photos of the 1945k III board around the SPR800E chip.

Development used Anthropic's Claude as a coding tool. All MAME scripts and
simulation harnesses are in each core's repository.
