# oxidized

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ytti/oxidized, licensed Apache-2.0, written in Ruby.

Evidence and recordings: https://argusic.com/subject/oxidized

## Pinned environment

- Project commit: `2cb5053566dfe4141aa02032d2cc8520be63c68a`
- Test commit: `2cb5053566dfe4141aa02032d2cc8520be63c68a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 10.1 | 2 | 2 | [run](https://argusic.com/run/2ade8bca-e21a-4084-809b-1313721f87fa) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Ruby not installed in container`
- 3 min: `charlock_holmes gem requires libicu-dev`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
