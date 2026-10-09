# ioBroker

**Verdict: runs.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ioBroker/ioBroker, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/iobroker

## Pinned environment

- Project commit: `e30d19e15377db6d251ea8b0eca60f00096bf3be`
- Test commit: `e30d19e15377db6d251ea8b0eca60f00096bf3be`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 9.8 to 14.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 12 | 9.8 | 2 | 2 | [run](https://argusic.com/run/1bf50548-e931-4a74-8310-c20fc91ef481) |
| 2 | pass | 100 | 7.5 | 14.9 | 3 | 3 | [run](https://argusic.com/run/adaf3235-d9ae-4aca-9a94-5b91dd5952b3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Installer requires root privileges for system operations (apt-get, useradd, write to /opt/iobroker, configure sudoers)`
- 1 min: `Container has Node.js 18.19.1, installer tooling requires Node.js 22+`

Attempt 2:

- 2 min: `Node.js v18 is too old for ioBroker (requires 22+). Had to download Node.js v22.14.0 from official tarball into $HOME/.local`
- 1 min: `sudo command not available in container`
- 3 min: `bash installer (dist/install.sh) cannot run , needs root for useradd, apt-get, mkdir in /opt. Cannot install system packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
