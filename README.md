# Wesker Slot

Wesker themed slot prototype.

## Play

Open `wesker.html` in a browser, or serve this folder with a local static server.

## Current Flow

- Normal / high-probability state draws CZ.
- CZ lasts 5G.
- CZ success starts AT.
- Ceiling is 500G.
- AT is game-count managed.
- Bell increases payout during AT.
- Rare roles add AT games.

## Prototype Setting Targets

These are rough simulation targets for the current prototype balance.

| Setting | Target rate | Simulated rough rate |
| --- | ---: | ---: |
| 1 | 88% | 87.4% |
| 2 | 92% | 91.9% |
| 3 | 96% | 95.5% |
| 4 | 102% | 101.1% |
| 5 | 108% | 109.8% |
| 6 | 116% | 117.1% |

Simulation assumes 3 medals in per game, including AT games.
AT bell payout is currently 9 medals, with rough AT net increase around +1.7 medals/G.

## Controls

- `BET`: start a game.
- `1 STOP`, `2 STOP`, `3 STOP`: stop each reel.
- `AUTO`: automatic play with automatic reel stops.
- `SKIP`: start/finish the current game quickly.
- Left menu buttons open stored data panels.
- Press `Esc` to close stored data.
