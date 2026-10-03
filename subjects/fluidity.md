# fluidity

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PrettyCoffee/fluidity, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/fluidity

## Pinned environment

- Project commit: `f502de59f4a652d667446e12adc09306bbe8c08e`
- Test commit: `f502de59f4a652d667446e12adc09306bbe8c08e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 6.5 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 6.6 | 2 | 2 | [run](https://argusic.com/run/376ff462-27b2-41fc-ba1f-2820234042a5) |
| 2 | fail | 80 | 8 | 6.5 | 2 | 2 | [run](https://argusic.com/run/1054cf59-7c8d-434b-90e8-2ce14f3f9259) |

## What was observed on a clean machine

Attempt 1:

- `@pretty-cozy/eslint-config@0.9.0-alpha.5 failed to install , its transitive dep @pretty-cozy/eslint-plugin does not exist in npm registry`
- `vite@7.3.1 requires Node >=20.19 but container has Node 18.19.1`

Attempt 2:

- 2 min: `npm install failed because @pretty-cozy/eslint-plugin@0.9.0-alpha.5 does not exist in the registry (dependency of @pretty-cozy/eslint-config)`
- 3 min: `Vite 7 and @vitejs/plugin-react 5 require Node >= 20, but only Node 18.19.1 is available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
