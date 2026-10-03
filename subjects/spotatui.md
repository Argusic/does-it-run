# spotatui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LargeModGames/spotatui, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/spotatui

## Pinned environment

- Project commit: `4348a70f33f117f07f23d40fd428f92f0f480b34`
- Test commit: `4348a70f33f117f07f23d40fd428f92f0f480b34`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.9 to 17.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 15.9 | 1 | 1 | [run](https://argusic.com/run/0fb78942-edb9-4504-925d-394e6a1b31ee) |
| 2 | pass | 100 | 11.2 | 17.8 | 2 | 2 | [run](https://argusic.com/run/daf82554-c00f-41aa-9cdd-e479809b7519) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `The full default build (librespot streaming, alsa-backend) requires libasound2-dev headers which are not installed in the container, and no root access is available to apt-get install them.`

Attempt 2:

- 0.2 min: `Rust toolchain not installed (no rustc/cargo in PATH)`
- 1 min: `default-features build failed: alsa-sys build.rs could not find alsa.pc (libasound2-dev not installed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
