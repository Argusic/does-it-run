# vps-audit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nuver-labs/vps-audit, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/vps-audit

## Pinned environment

- Project commit: `57c323d46b48026740f0b35b9bad6cd6127c757b`
- Test commit: `57c323d46b48026740f0b35b9bad6cd6127c757b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.4 to 2.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0 | 2.4 | 1 | 1 | [run](https://argusic.com/run/6f7a3b67-2446-4cfd-a739-f884ba437060) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Debian version parsing fails on non-numeric /etc/debian_version (e.g. 'trixie/sid')`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
