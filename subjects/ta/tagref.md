# tagref

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/stepchowfun/tagref, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/tagref

## Pinned environment

- Project commit: `4894b87986ca07954c5edc2f3c1def4d01025a6f`
- Test commit: `4894b87986ca07954c5edc2f3c1def4d01025a6f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2 to 2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 2 | 1 | 1 | [run](https://argusic.com/run/24a96a4d-8a6f-4022-87c5-18ae3c10dec8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Official install.sh failed on first run: target dir missing, mv failed, then the script hit a sudo branch needing a tty (cannot open /dev/tty) and exited with "Unable to install the binary"`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
