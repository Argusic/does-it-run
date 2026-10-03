# lazygit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jesseduffield/lazygit, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/lazygit

## Pinned environment

- Project commit: `3f6be3b3ee7b69c0dbed429669134fd04e1e9e35`
- Test commit: `3f6be3b3ee7b69c0dbed429669134fd04e1e9e35`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 8.3 to 12.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 12.7 | 1 | 1 | [run](https://argusic.com/run/ccc865a3-3f4b-4319-aa32-c923ec417a1c) |
| 2 | pass | 100 | 5 | 8.3 | 3 | 3 | [run](https://argusic.com/run/e4dd445e-3cb8-49d6-a507-780750dad0e6) |
| 3 | pass | 100 | 3 | 11.5 | 1 | 1 | [run](https://argusic.com/run/2a2771e2-62a9-4826-b443-e8408ac15120) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `NO_COLOR env var causes gookit/color to suppress ANSI output in style tests`

Attempt 2:

- 3 min: `go not installed`
- 1 min: `just not installed`
- 15 min: `11 color-rendering tests fail with NO_COLOR=1 env set`

Attempt 3:

- 5 min: `style tests fail under NO_COLOR=1 because gookit/color disables ANSI output when Enable=false`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
