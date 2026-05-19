# Wesker Slot

Wesker themed slot prototype.

## Play

Open `wesker.html` in a browser, or serve this folder with a local static server.

Open `wesker_spec_preview.html` to preview the current specification, setting targets, role probabilities, and reel strips.

Open `wesker_machine.html` to play the current machine-style prototype with bonus, RUSH, Harakiri Challenge, Harakiri Drive, and comeback state flow.

## Current Flow

- Normal / high-probability state draws CZ.
- CZ lasts 5G.
- CZ success starts AT.
- Ceiling is 500G.
- AT is game-count managed.
- Bell increases payout during AT.
- Rare roles add AT games.

The target Wesker game specification is stored in `Documents/WESKER_SPEC.md`.

## Target Wesker Spec

- AT net increase is about 7.2 pt/G.
- Revolution Bonus is a pseudo BIG: 50G + alpha, average about 470 pt, 666 pt payout guarantees RUSH.
- After 666 pt in Revolution Bonus, remaining games run V-stock lottery.
- Decisive Battle Bonus is a pseudo REG: bell navigation 8 times + battle, average about 110 pt, battle success about 35%.
- Revolution RUSH has 75% continuation, 10 to 100G + alpha initial games, average about 1320 pt.
- Super Revolution RUSH has 90% continuation, favored initial games, average about 2190 pt.
- Reaching the 4th Revolution RUSH set upgrades to Super Revolution RUSH.
- Harakiri Challenge is a 3G high-speed continuation judgment after RUSH, with about 77% after Revolution RUSH and about 90% after Super Revolution RUSH, including the 66G comeback lottery.
- Harakiri Drive is a game-count add special zone with three-digit add expectation.
- After bonus or RUSH ends, the machine has an internal 66G RUSH comeback state.

## Prototype Setting Targets

These are rough simulation targets for the current prototype balance.

| Setting | Target rate | Tuned rough rate |
| --- | ---: | ---: |
| 1 | 85% | 85.5% |
| 2 | 90% | 90.3% |
| 3 | 95% | 95.4% |
| 4 | 101% | 101.4% |
| 5 | 108% | 107.9% |
| 6 | 115% | 115.4% |

Simulation assumes 3 medals in per game, including AT games.
AT bell payout is currently 9 medals, with rough AT net increase around +1.7 medals/G.

## Controls

- `BET`: start a game.
- `1 STOP`, `2 STOP`, `3 STOP`: stop each reel.
- `AUTO`: automatic play with automatic reel stops.
- `SKIP`: start/finish the current game quickly.
- Left menu buttons open stored data panels.
- Press `Esc` to close stored data.
