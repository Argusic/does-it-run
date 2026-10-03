# magic-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/21st-dev/magic-mcp, licensed ISC, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/magic-mcp

## Pinned environment

- Project commit: `6e5a43d3621442a450948864a74396d206b23c65`
- Test commit: `6e5a43d3621442a450948864a74396d206b23c65`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 3 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.05 | 4.2 | 0 | 0 | [run](https://argusic.com/run/68d8064e-d734-43aa-8c1d-058ce5742c27) |
| 2 | pass with mocks | 92 | 3 | 3.5 | 0 | 0 | [run](https://argusic.com/run/86619535-3308-486f-acc7-32f859db4e83) |
| 3 | pass with mocks | 92 | 1.5 | 3 | 0 | 0 | [run](https://argusic.com/run/5557a98b-17f0-456f-96ef-35f3393bbc88) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
