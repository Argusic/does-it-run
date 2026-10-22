# claude-remotion-skill

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/haidrrrry/claude-remotion-skill, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/claude-remotion-skill

## Pinned environment

- Project commit: `1dcbe5e3fc6cf970bd10d3cc05f0a8a5d19d0383`
- Test commit: `1dcbe5e3fc6cf970bd10d3cc05f0a8a5d19d0383`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 1 | 4.2 | 2 | 1 | [run](https://argusic.com/run/a7632f64-6405-47d0-91e6-808c476fa6fc) |

## What was observed on a clean machine

Attempt 1:

- `/bin/sh: 1: time: not found`
- 1 min: `scripts/build-skill.sh needs zip, which is not installed and cannot be installed without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
