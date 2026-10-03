# gecco

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xtuhcy/gecco, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/gecco

## Pinned environment

- Project commit: `e1f32e1c437b783ac019754d1b3c4401b67572ba`
- Test commit: `e1f32e1c437b783ac019754d1b3c4401b67572ba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.8 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.7 | 4.8 | 2 | 2 | [run](https://argusic.com/run/9aba238c-ef80-4148-a04b-732c45cfd2aa) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Java and Maven not available in container`
- 0.5 min: `cglib library incompatible with JDK 17 module system`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
