# canonry

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Canonry/canonry, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/canonry

## Pinned environment

- Project commit: `bd245fdfebf871aed492ec7e4d2d4204db76cfc0`
- Test commit: `bd245fdfebf871aed492ec7e4d2d4204db76cfc0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.7 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 18.7 | 4 | 4 | [run](https://argusic.com/run/f97704dd-ee7b-4354-a48d-dc0011d636cc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm not found in container`
- 3 min: `Node v18.19.1 too old (requires >=26.12.1)`
- 1 min: `.npmrc prefix setting conflicted with nvm`
- `sqlite3 CLI binary not found, 2 tests skip`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
