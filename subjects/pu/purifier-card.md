# purifier-card

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/denysdovhan/purifier-card, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/purifier-card

## Pinned environment

- Project commit: `353874df2598d39885c9f3d6aae9d67cb9e61234`
- Test commit: `353874df2598d39885c9f3d6aae9d67cb9e61234`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.6 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 10.6 | 2 | 2 | [run](https://argusic.com/run/89af6672-ce13-4453-aad2-af73fe480bfa) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `script scripts/validate-i18n (ES module) failed: Cannot use import statement outside a module because package.json lacked "type": "module"`
- 3 min: `Rollup build failed: ReferenceError: crypto is not defined (serialize-javascript@7.0.5 via @rollup/plugin-terser@1.0.0 requires Node >= 20; container has Node 18)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
