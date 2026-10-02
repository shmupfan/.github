<img src="logo.png" width="128" align="right" alt="shmupfan logo: a pixel-art fighter firing a laser through a bullet curtain">

# shmupfan

MiSTer FPGA arcade cores and tools, mostly for shoot 'em ups.

## Cores

| Core | Games | Get it |
|---|---|---|
| [Hyper Duel](https://github.com/searchsolved/Arcade-HyperDuel_MiSTer) | Hyper Duel (Technosoft, 1993). First FPGA implementation of the Imagetek I4220 video chip | In the official MiSTer distribution: just run Update All. Also on [MiSTer-devel](https://github.com/MiSTer-devel/Arcade-HyperDuel_MiSTer) |
| [Dooyong](https://github.com/shmupfan/Arcade-Dooyong_MiSTer) | The Last Day, Gulf Storm, Pollux, Flying Tiger, Blue Hawk, Sadari, Gun Dealer '94, Super-X, R-Shark, Pop Bingo | Update All with the shmupfan database (below) |

## Update All

New cores land in the [shmupfan database](https://github.com/shmupfan/Distribution).
Add these two lines to `/media/fat/downloader.ini` once, and every Update All
run installs and updates them:

```ini
[shmupfan]
db_url = https://raw.githubusercontent.com/shmupfan/Distribution/main/db.json
```

## Shmup Deck

[Shmup Deck](https://github.com/shmupfan/shmup-deck) is a flyer-wall launcher
for shoot 'em ups on the MiSTer. Open it on your phone, tap a flyer, and the
MiSTer loads the game. It runs on the MiSTer itself and covers 294 shooters on
106 arcade boards.
