# RL Generalization-Gap — Results Summary

_Generated 2026-06-20 21:52 · FULL run · 8 seeds_

## Test-return IQM (95% CI) and probability of improvement vs baseline

| Condition | Test IQM | 95% CI | P(improve > base) |
|---|---|---|---|
| baseline|- | -0.800 | [-0.800, -0.800] | — |
| levels|2 | -0.800 | [-0.800, -0.800] | 0.45 |
| levels|4 | -0.800 | [-0.800, -0.800] | 0.45 |
| levels|16 | -0.800 | [-0.800, -0.800] | 0.45 |
| levels|64 | -0.800 | [-0.800, -0.800] | 0.50 |
| levels|256 | +0.137 | [+0.055, +0.223] | 0.70 |
| aug|shift | -0.309 | [-0.425, -0.198] | 0.64 |
| aug|cutout | -0.800 | [-0.800, -0.800] | 0.49 |
| reg|l2 | -0.800 | [-0.800, -0.796] | 0.55 |
| reg|0.1 | -0.800 | [-0.800, -0.800] | 0.51 |
| width|x2 | -0.800 | [-0.800, -0.800] | 0.49 |

## Mean train / test / gap

| Condition | Setting | Train | Test | Gap |
|---|---|---|---|---|
| aug | cutout | +0.886 | -0.647 | +1.533 |
| aug | shift | +0.903 | -0.114 | +1.018 |
| baseline | - | +0.896 | -0.595 | +1.491 |
| levels | 16 | +0.895 | -0.769 | +1.664 |
| levels | 2 | +0.830 | -0.760 | +1.590 |
| levels | 256 | +0.903 | +0.109 | +0.794 |
| levels | 4 | +0.870 | -0.762 | +1.632 |
| levels | 64 | +0.896 | -0.595 | +1.491 |
| reg | 0.1 | +0.886 | -0.570 | +1.456 |
| reg | l2 | +0.896 | -0.404 | +1.300 |
| width | x2 | +0.903 | -0.618 | +1.521 |