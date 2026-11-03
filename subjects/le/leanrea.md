# leanrea

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aicodeking/leanrea, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/leanrea

## Pinned environment

- Project commit: `09ba4aa0217f82cd880f855a60b877f59f39b22b`
- Test commit: `09ba4aa0217f82cd880f855a60b877f59f39b22b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 0.1 | 3.2 | 1 | 1 | [run](https://argusic.com/run/87f4bbeb-90c8-43e4-b55e-d1cbb32bf0c9) |
| 2 | fail | 50 | 2 | 2 | 1 | 1 | [run](https://argusic.com/run/ac4ec8dd-7d4a-47c0-a6f8-e4f3a16879b4) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `npx skills add aicodeking/leanrea fails: Node.js v18 does not meet the >=22.20.0 requirement of the skills@1.7.4 npm package`

Attempt 2:

- 2 min: `skills CLI (npx skills add) requires Node >= 22.20.0, but system Node is v18.19.1; downloaded Node v22.14.0 as a workaround and the install worked`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
