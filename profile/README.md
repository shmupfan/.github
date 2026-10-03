# shmupfan

MiSTer FPGA arcade cores for games with no existing core, mostly shoot 'em ups.
Every core is verified against MAME frame by frame and checked against hardware
documentation; see the [accuracy method](https://github.com/shmupfan/.github/blob/main/ACCURACY.md).

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
| [Dooyong](https://github.com/shmupfan/Arcade-Dooyong_MiSTer) | The Last Day, Gulf Storm, Pollux, Flying Tiger, Blue Hawk, Sadari, Gun Dealer '94, Super-X, R-Shark, Pop Bingo | shmupfan database |
| [Hyper Duel](https://github.com/searchsolved/Arcade-HyperDuel_MiSTer) | Hyper Duel (Technosoft, 1993); first FPGA implementation of the Imagetek I4220 video chip | Official MiSTer distribution |

In development: 1945k III / Solite Spirits, Final Star Force (Tecmo 16), Super
Real Darwin / Last Mission / Gondomania (Data East DEC8), Twin Falcons / Turtle
Ship / Dyger.

## Shmup Deck

[Shmup Deck](https://github.com/shmupfan/shmup-deck) is a flyer-wall launcher
that runs on the MiSTer: open it on a phone, tap a flyer, and the game loads.
It covers 294 shooters on 106 arcade boards.
