# shmupfan

MiSTer FPGA arcade cores for games with no existing core, mostly shoot 'em ups.

Read how I [strive for accuracy](https://github.com/shmupfan/.github/blob/main/ACCURACY.md).

## Install

Add these two lines to `/media/fat/downloader.ini`, then run Update All. New
cores and updates arrive with every run.

```ini
[shmupfan]
db_url = https://raw.githubusercontent.com/shmupfan/Distribution/main/db.json
```

## Cores

| Core | Games | Install |
|---|---|---|
| [1945k III](https://github.com/shmupfan/Arcade-1945kIII_MiSTer) | 1945k III, Solite Spirits, '96 Flag Rally | shmupfan database |
| [Dooyong](https://github.com/shmupfan/Arcade-Dooyong_MiSTer) | The Last Day, Gulf Storm, Pollux, Flying Tiger, Blue Hawk, Sadari, Gun Dealer '94, Super-X, R-Shark, Pop Bingo | shmupfan database |
| [DEC8](https://github.com/shmupfan/Arcade-DEC8_MiSTer) | Last Mission, Gondomania, SRD: Super Real Darwin | shmupfan database |
| [Tecmo 16](https://github.com/shmupfan/Arcade-Tecmo16_MiSTer) | Final Star Force, Riot, Ganbare Ginkun | shmupfan database |
| [Taito G-NET](https://github.com/shmupfan/Arcade-TaitoGNET_MiSTer) (alpha) | Ray Crisis, Psyvariar -Medium Unit-, Psyvariar -Revision-, Shikigami no Shiro, Night Raid, XII Stag, Chaos Heat, Super Puzzle Bobble and 14 more. Game files are made from your MAME CHDs with the [converter](https://gnet-converter.pages.dev) | shmupfan database |
| [Hyper Duel](https://github.com/searchsolved/Arcade-HyperDuel_MiSTer) | Hyper Duel (Technosoft, 1993); first FPGA implementation of the Imagetek I4220 video chip | Official MiSTer distribution |

In development: Twin Falcons / Turtle Ship / Dyger.

## Shmup Deck

[Shmup Deck](https://github.com/shmupfan/shmup-deck) is a flyer-wall launcher
that runs on the MiSTer: open it on a phone, tap a flyer, and the game loads.
New shmupfan cores are added to it as they release.
