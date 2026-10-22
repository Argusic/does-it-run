# daffodil

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/graycoreio/daffodil, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/daffodil

## Pinned environment

- Project commit: `538c062d742958634cca3f166cc44fbd009a6b87`
- Test commit: `538c062d742958634cca3f166cc44fbd009a6b87`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 50.3 to 50.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 49 | 50.3 | 3 | 3 | [run](https://argusic.com/run/a52cc84c-044b-4f58-8727-fa69980f3afc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node is v18.19.1 but .nvmrc requires 24.19 and Angular 21 needs Node >=20`
- 12 min: `nx build process died mid-stream (log ended with no summary)`
- 25 min: `Karma tests need Chrome but no browser is installed in the container; ChromeHeadless launcher lacks --no-sandbox and crashes in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
