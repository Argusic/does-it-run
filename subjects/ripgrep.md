# ripgrep

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BurntSushi/ripgrep, licensed Unlicense, written in Rust.

Evidence and recordings: https://argusic.com/subject/ripgrep

## Pinned environment

- Project commit: `3fce3b5bb0236da2df6d99672afb8a719642eca7`
- Test commit: `3fce3b5bb0236da2df6d99672afb8a719642eca7`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 1.8 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 13 | 2 | 2 | [run](https://argusic.com/run/6d31dab9-a282-47fe-b157-fc0e54f29727) |
| 2 | pass | 100 | 7.4 | 1.8 | 0 | 0 | [run](https://argusic.com/run/65339b30-b80b-48e7-bcae-8e4ad824dbdf) |
| 3 | pass | 100 | 1.2 | 3.1 | 0 | 0 | [run](https://argusic.com/run/6ec0f4cc-c2f5-4b6f-a569-67271dd3b17d) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `rustc: not found`
- 2 min: `linker 'cc' not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
