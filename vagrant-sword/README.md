# Vagrant Sword charge timing

Nameless / Bellstrike Splendor. How long you actually have to hold R to get
three blasts instead of one.

**Short answer: hold 87 frames (1450 ms). The real threshold is around
1411 ms, but 85 frames fails a third of the time.**

## Charge timeline

From the moment R goes down, at 60 fps:

| event | frames | ms |
|---|---|---|
| 1st ding | 24 | 395 |
| 3-blast threshold | ~85 | ~1411 |
| 2nd ding | 93 | 1555 |
| auto-cast at max charge | 127 | 2120 |

The usual advice to release after the second ding is safe but slow - the
threshold sits about 144 ms *before* that ding. The attack also fires itself
at max charge whether or not you are still holding, so holding past 2120 ms
gains nothing.

## Where the threshold is

31 isolated casts, music muted, outcome scored from post-release audio and
spot-checked frame by frame:

| frames | hold (ms) | n | 3-blast | rate |
|---|---|---|---|---|
| 78-84 | 1300-1400 | 17 | 0 | 0.00 |
| 85 | 1417 | 6 | 4 | 0.67 |
| 87-92 | 1450-1533 | 8 | 8 | 1.00 |

Nothing below 85 frames has ever worked. 85 works about two times in three.
87 and above has never failed.
