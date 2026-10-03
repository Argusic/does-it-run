# sh

**Verdict: runs with mocks.** Argusic Score 80.6 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kejilion/sh, licensed Apache-2.0, written in Shell.

Evidence and recordings: https://argusic.com/subject/sh

## Pinned environment

- Project commit: `478f322a1097b4474a05aaf7fe0d54b05bd68aa9`
- Test commit: `478f322a1097b4474a05aaf7fe0d54b05bd68aa9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 25.7 to 25.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 80.57 | 1 | 25.7 | 7 | 3 | [run](https://argusic.com/run/f614c6e6-810b-4581-a262-37b4bb8868c9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `ssh-keygen not found`
- 1 min: `xxd not found`
- 2 min: `npm install -g @tobilu/qmd EACCES`
- 2 min: `disk_management path security check requires root uid`
- 1 min: `system_tuning needs root for OpenSSH config`
- 1 min: `web_certificate needs root for file ownership checks`
- 1 min: `http_nginx_live needs NGINX_BIN env var`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
