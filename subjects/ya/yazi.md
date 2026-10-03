# yazi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sxyazi/yazi, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/yazi

## Pinned environment

- Project commit: `5f901b886b14de1f17460b6e52e9de5d67f8aba9`
- Test commit: `5f901b886b14de1f17460b6e52e9de5d67f8aba9`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 15.9 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 15.9 | 2 | 2 | [run](https://argusic.com/run/ff1bc876-d295-4213-a284-74c109e7da22) |
| 2 | pass | 100 | 15 | 22.4 | 1 | 1 | [run](https://argusic.com/run/7782b1a4-c3a5-4646-a9ce-beb8f5a7ec80) |
| 3 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/d39dbef9-043c-41e5-9f89-e2ddbf384c9e) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `No C compiler or Rust toolchain installed in the container`
- 2 min: `No pkg-config binary available`

Attempt 2:

- 1 min: `Rust toolchain not installed in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
