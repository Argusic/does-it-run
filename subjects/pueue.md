# pueue

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Nukesor/pueue, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/pueue

## Pinned environment

- Project commit: `b3a2077ddc57d956cdf77e8b767831bc3d4597c7`
- Test commit: `b3a2077ddc57d956cdf77e8b767831bc3d4597c7`
- Worker image digests: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`, `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 9.7 to 42 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 14.3 | 1 | 1 | [run](https://argusic.com/run/ef3f7472-4d69-4dda-a9f7-6ba227ed3231) |
| 2 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/e627b8fb-7532-49df-a4ae-073a597fe4c1) |
| 3 | pass | 100 | 2 | 9.7 | 1 | 1 | [run](https://argusic.com/run/5c92fb61-01b1-48af-8c3b-5ae41a1c741c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Snapshot tests 'group::colored' and 'log::colored' failed because the container's TERM=dumb terminal doesn't support 256-color ANSI codes. The snapshots expected \x1b[38;5;10m (256-color green) and \x1b[39m (default fg), but the actual outp`

Attempt 3:

- `2 integration tests (client::integration::group::colored, client::integration::log::colored) failed under NO_COLOR/TERM=dumb env due to ANSI color code mismatch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
