# cortex

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cortex-docs/cortex, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cortex

## Pinned environment

- Project commit: `0aa5e33cddc440e8ad7efa2de2bf9fd9e8fc8ce9`
- Test commit: `0aa5e33cddc440e8ad7efa2de2bf9fd9e8fc8ce9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.9 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 5.9 | 1 | 1 | [run](https://argusic.com/run/5ca83fb0-3b78-45c2-bfd5-ccb9e0cdb6f6) |
| 2 | pass | 100 | 11 | 12.4 | 3 | 3 | [run](https://argusic.com/run/08a04e82-5e75-4779-8196-67c1df3011b7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Pre-installed Node.js v18 too old (project requires >=20).`

Attempt 2:

- 10 min: `Node.js v18.19.1 in container , project requires >=20.0.0`
- `docs-ui builds fail: Next.js >=16 requires Node >=20.9.0`
- `docs-site build fails: same Next.js Node requirement`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
