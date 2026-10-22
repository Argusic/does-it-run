# openqodex

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openqodex/openqodex, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openqodex

## Pinned environment

- Project commit: `549d3301702a739d62bd7296e2b9c94ce17af1ce`
- Test commit: `549d3301702a739d62bd7296e2b9c94ce17af1ce`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 12.7 to 52.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 52.6 | 0 | 0 | [run](https://argusic.com/run/195de77b-bb45-43f2-84ac-30ff23f4b4ab) |
| 2 | pass with mocks | 92 | 11 | 12.7 | 4 | 4 | [run](https://argusic.com/run/6a96bd01-2f76-4de7-a685-7f88764dd142) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node in container was 18.19.1 but the repo needs 22+`
- 1 min: `pnpm not installed`
- 8 min: `e2e review-target partial-clone test failed: it asserts git >= 2.44 behavior but git here is 2.43.0; the CLI printed its documented old-git message`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
