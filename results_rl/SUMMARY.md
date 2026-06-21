# RL Generalization-Gap — Results Summary

_Generated 2026-06-21 17:03 · FULL run · 8 seeds_

**How to read this.** Every agent trains to near-optimal on its *training* levels; the question is how it does on *held-out* levels. `Solved` = fraction of held-out levels the greedy policy reaches the goal on (this metric does not saturate). `Test IQM` = interquartile mean of held-out return (robust, but floors at the timeout penalty when most levels are unsolved). `Gap` = train − test return. `P(improve)` = probability a random (seed, level) beats the baseline.

## Ranked by held-out success rate

| Condition | Solved | 95% CI | Test IQM | P(improve) |
|---|---|---|---|---|
| levels|256 | 57% | [54%, 60%] | +0.289 | 0.69 |
| levels|192 | 52% | [49%, 56%] | +0.138 | 0.67 |
| levels|128 | 37% | [32%, 42%] | -0.386 | 0.60 |
| aug|shift | 36% | [32%, 40%] | -0.425 | 0.59 |
| reg|l2 | 35% | [31%, 39%] | -0.447 | 0.59 |
| levels|96 | 29% | [25%, 34%] | -0.651 | 0.56 |
| baseline|- | 17% | [14%, 20%] | -0.800 | — |
| levels|64 | 17% | [14%, 20%] | -0.800 | 0.50 |
| reg|0.1 | 12% | [10%, 14%] | -0.800 | 0.48 |
| width|x2 | 12% | [9%, 15%] | -0.800 | 0.48 |
| aug|cutout | 10% | [8%, 11%] | -0.800 | 0.46 |
| levels|4 | 3% | [2%, 4%] | -0.800 | 0.43 |
| levels|16 | 2% | [2%, 3%] | -0.800 | 0.43 |
| levels|2 | 2% | [1%, 3%] | -0.800 | 0.43 |

## Mean train / test / gap (return)

| Condition | Setting | Train | Test | Solved | Gap |
|---|---|---|---|---|---|
| aug | cutout | +0.896 | -0.631 | 10% | +1.527 |
| aug | shift | +0.910 | -0.173 | 36% | +1.083 |
| baseline | - | +0.906 | -0.503 | 17% | +1.409 |
| levels | 128 | +0.914 | -0.154 | 37% | +1.068 |
| levels | 16 | +0.920 | -0.765 | 2% | +1.684 |
| levels | 192 | +0.920 | +0.110 | 52% | +0.811 |
| levels | 2 | +0.830 | -0.765 | 2% | +1.595 |
| levels | 256 | +0.927 | +0.185 | 57% | +0.741 |
| levels | 4 | +0.708 | -0.749 | 3% | +1.457 |
| levels | 64 | +0.906 | -0.503 | 17% | +1.409 |
| levels | 96 | +0.912 | -0.288 | 29% | +1.200 |
| reg | 0.1 | +0.905 | -0.590 | 12% | +1.495 |
| reg | l2 | +0.920 | -0.185 | 35% | +1.104 |
| width | x2 | +0.926 | -0.590 | 12% | +1.516 |