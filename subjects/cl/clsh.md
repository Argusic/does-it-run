# clsh

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/my-claude-utils/clsh, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/clsh

## Pinned environment

- Project commit: `986b8b866f9d9203d5686ee46db36716c54c9e81`
- Test commit: `986b8b866f9d9203d5686ee46db36716c54c9e81`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 1.7 to 2.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 1.7 | 0 | 0 | [run](https://argusic.com/run/f893cc0a-7f4c-4980-afd8-47f710cbfa36) |
| 2 | pass | 100 | 1 | 2.3 | 1 | 1 | [run](https://argusic.com/run/8b3ce6dd-f281-4f17-b41d-8a3b036c117a) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js v18 too old (needs >=20)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
