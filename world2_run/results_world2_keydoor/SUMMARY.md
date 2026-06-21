# Generalization-Gap Results — `world2_keydoor`

_Generated 2026-06-21 23:03 · FULL run · 8 seeds_

**How to read this.** Every agent trains to near-optimal on its *training* levels; the question is held-out performance. `Solved` = fraction of held-out levels completed (success flag, not return>0), which does not saturate. `IQM` = interquartile mean of held-out return. `Gap` = train-test return. `P(impr)` = probability a random (seed,level) return beats baseline.

## Ranked by held-out success rate

| Condition | Solved | 95% CI | IQM(ret) | P(impr) |
|---|---|---|---|---|
| levels|256 | 57% | [53%, 60%] | +0.152 | 0.65 |
| levels|192 | 55% | [53%, 57%] | +0.084 | 0.64 |
| levels|128 | 47% | [43%, 50%] | -0.249 | 0.60 |
| reg|l2 | 44% | [40%, 47%] | -0.358 | 0.59 |
| levels|96 | 35% | [31%, 40%] | -0.700 | 0.55 |
| aug|shift | 32% | [30%, 36%] | -0.808 | 0.54 |
| baseline|- | 25% | [22%, 28%] | -1.100 | — |
| levels|64 | 25% | [22%, 28%] | -1.100 | 0.50 |
| reg|0.1 | 21% | [18%, 25%] | -1.100 | 0.48 |
| width|x2 | 20% | [15%, 25%] | -1.100 | 0.48 |
| aug|cutout | 17% | [14%, 21%] | -1.100 | 0.46 |
| levels|16 | 1% | [0%, 1%] | -1.100 | 0.38 |
| levels|2 | 0% | [0%, 1%] | -1.100 | 0.38 |
| levels|4 | 0% | [0%, 1%] | -1.100 | 0.38 |

## Mean train / test / gap

| Condition | Setting | Train | Test | Solved | Gap |
|---|---|---|---|---|---|
| aug | cutout | +0.856 | -0.757 | 17% | +1.613 |
| aug | shift | +0.814 | -0.450 | 32% | +1.264 |
| baseline | - | +0.848 | -0.602 | 25% | +1.451 |
| levels | 128 | +0.848 | -0.169 | 47% | +1.018 |
| levels | 16 | +0.805 | -1.083 | 1% | +1.888 |
| levels | 192 | +0.846 | -0.002 | 55% | +0.848 |
| levels | 2 | +0.628 | -1.095 | 0% | +1.723 |
| levels | 256 | +0.807 | +0.032 | 57% | +0.775 |
| levels | 4 | +0.804 | -1.095 | 0% | +1.899 |
| levels | 64 | +0.848 | -0.602 | 25% | +1.451 |
| levels | 96 | +0.842 | -0.397 | 35% | +1.238 |
| reg | 0.1 | +0.810 | -0.675 | 21% | +1.485 |
| reg | l2 | +0.872 | -0.223 | 44% | +1.095 |
| width | x2 | +0.864 | -0.699 | 20% | +1.563 |