# RL Generalization-Gap — Results Summary

_Generated 2026-06-20 19:31 · SMOKE run · 2 seeds_

## Test-return IQM (95% CI) and probability of improvement vs baseline

| Condition | Test IQM | 95% CI | P(improve > base) |
|---|---|---|---|
| baseline|- | -0.360 | [-0.360, -0.360] | — |
| levels|16 | -0.360 | [-0.360, -0.360] | 0.50 |
| aug|shift | -0.360 | [-0.360, -0.360] | 0.53 |
| reg|l2 | -0.360 | [-0.360, -0.360] | 0.59 |
| width|x2 | -0.360 | [-0.360, -0.360] | 0.50 |

## Mean train / test / gap

| Condition | Setting | Train | Test | Gap |
|---|---|---|---|---|
| aug | shift | -0.030 | -0.191 | +0.161 |
| baseline | - | +0.788 | -0.276 | +1.063 |
| levels | 16 | +0.385 | -0.276 | +0.661 |
| reg | l2 | +0.624 | -0.027 | +0.651 |
| width | x2 | +0.786 | -0.276 | +1.062 |