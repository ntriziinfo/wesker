# Wesker Slot Specification

## Core Values

- AT net increase: about 7.2 pt/G.
- Ceiling: 500G.
- Main route: normal / high-probability state -> CZ / bonus route -> RUSH.
- Payout unit is managed as `pt` in the prototype.

## Revolution Bonus

Revolution Bonus is a pseudo BIG.

- Base games: 50G + alpha.
- Average payout: about 470 pt.
- If total payout reaches 666 pt, Revolution RUSH is guaranteed.
- Rare roles can trigger game-count decrement stop.
- After 666 pt is reached, remaining games run V-stock lottery.

## Decisive Battle Bonus

Decisive Battle Bonus is a pseudo REG.

- Bell navigation: 8 times + battle.
- Average payout: about 110 pt.
- Battle victory leads to Revolution RUSH.
- Battle success rate: about 35%.

## Revolution RUSH

Revolution RUSH is the normal AT.

- Continuation rate: 75%.
- Net increase: about 7.2 pt/G.
- Initial games: 10 to 100G + alpha.
- Entry set is expected to be 20G or more.
- Average payout: about 1320 pt.
- Type: continuation loop + game-count add + set-stock.
- Reaching the 4th Revolution RUSH set upgrades to Super Revolution RUSH.

## Super Revolution RUSH

Super Revolution RUSH is the upper AT.

- Continuation rate: 90%.
- Net increase: about 7.2 pt/G.
- Initial games: 10 to 100G + alpha.
- Initial game lottery is favored over Revolution RUSH by about 1.5x.
- Average payout: about 2190 pt.
- Type: continuation loop + game-count add + set-stock.

## Implementation Notes

- Current HTML prototype still uses the earlier simple CZ -> AT game-count flow.
- This document is the current target specification for the next balance and state-machine rewrite.
- Bonus/RUSH payout displays should use `pt` consistently unless the design intentionally switches to medals.
