# open-code-review

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alibaba/open-code-review, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/open-code-review

## Pinned environment

- Project commit: `a694be568d9b9a935b2ba11a867d5a91d7ffd833`
- Test commit: `a694be568d9b9a935b2ba11a867d5a91d7ffd833`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 13.5 to 26.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 36.68 | 13.5 | 0 | 0 | [run](https://argusic.com/run/f6ea56c9-37cd-4e55-9a70-741a791e60dc) |
| 2 | pass with mocks | 92 | 5 | 26.3 | 1 | 1 | [run](https://argusic.com/run/abe1d8fa-f329-4476-9e8b-1f70d44ed366) |
| 3 | pass | 100 | 15 | 15.3 | 2 | 2 | [run](https://argusic.com/run/73cfe91b-7fe5-48d4-ad61-41f20c978648) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go 1.25.5 not installed in container`

Attempt 3:

- 5 min: `Go toolchain not installed in container`
- 1 min: `npm install -g fails with EACCES (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
