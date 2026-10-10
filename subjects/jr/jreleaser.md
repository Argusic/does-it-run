# jreleaser

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jreleaser/jreleaser, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/jreleaser

## Pinned environment

- Project commit: `99949bedac822a701e1c34950b71c164e98df18a`
- Test commit: `99949bedac822a701e1c34950b71c164e98df18a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 9.7 to 28.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 9.7 | 0 | 0 | [run](https://argusic.com/run/34155c5b-9967-449d-b601-579638b7e04b) |
| 2 | pass | 100 | 28 | 28.3 | 3 | 3 | [run](https://argusic.com/run/b4e58a6d-1a6e-400b-a18d-ef166fdc2c9b) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `no java/JAVA_HOME in container`
- 1 min: `/work not writable for tool install`
- 1 min: `jreleaser init --format yaml rejected (Unsupported file format; must be yml|toml|json)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
