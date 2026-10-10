# omarchy

**Verdict: runs.** Argusic Score 89.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/omacom/omarchy, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/omarchy

## Pinned environment

- Project commit: `c352b62d67456f56ca898d0e23effc1b20c25ca6`
- Test commit: `c352b62d67456f56ca898d0e23effc1b20c25ca6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 73.8 to 73.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 89.33 | 0 | 73.8 | 15 | 7 | [run](https://argusic.com/run/6fa724c2-dba9-4618-aebe-51c0b4184ecd) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Template renderer lost newlines by using awk's RT in a getline loop`
- 2 min: `ASCII test expected Hi=18 columns, font now produces 30`
- 4 min: `Grok migration uses mise unuse -y -g but tests expected unuse -g`
- 2 min: `hw-hybrid-gpu test PATH missing $ROOT/bin`
- 2 min: `launch-browser test PATH missing $ROOT/bin`
- 2 min: `mise not installed in container (rootless)`
- 1 min: `socat not installed in container (rootless)`
- 1 min: `lua5.4 not installed in container (rootless)`
- 1 min: `magick (ImageMagick 7) not installed; only convert-im6.q16 available`
- 1 min: `updatedb not installed in container`
- 1 min: `timedatectl fails (no systemd as PID 1 in container)`
- 1 min: `plymouth test needs root-owned directory for publishing validation`
- 1 min: `neovim migration uses vercmp which is not installed`
- 1 min: `omarchy-sudo test needs root-like environment`
- 1 min: `omarchy-provision-user needs mise and update-desktop-database`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
