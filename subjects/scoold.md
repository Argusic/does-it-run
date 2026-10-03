# scoold

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Erudika/scoold, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/scoold

## Pinned environment

- Project commit: `16bf78802aa96d41764b3c78d2371cea6e611f80`
- Test commit: `16bf78802aa96d41764b3c78d2371cea6e611f80`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 21.5 to 34.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 33 | 34.9 | 6 | 6 | [run](https://argusic.com/run/e953d3b6-ebab-4332-afad-ffa8706c1a2c) |
| 2 | fail | 20 | n/a | 21.5 | 0 | 0 | [run](https://argusic.com/run/73534a87-26a3-40bd-9fdc-20b82db72690) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Java 21 not available in container, had to download Adoptium JDK 21 manually`
- 2 min: `Maven not available in container, had to download manually`
- 1 min: `Spring Boot 4.x requires Java 21, JDK 17 caused compilation error (release version 21 not supported)`
- 5 min: `Para backend not running, needed to download and start Para 1.55.2 server`
- 2 min: `Scoold autoinit config key mismatch (used autoinit.para_root_secret_key instead of autoinit.root_app_secret_key)`
- 1 min: `Background Java processes being killed when shell session ends`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
