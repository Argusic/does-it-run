# Purse

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/drduh/Purse, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/purse

## Pinned environment

- Project commit: `9b2f643cdd2146457214d3638dac3b73071921a2`
- Test commit: `9b2f643cdd2146457214d3638dac3b73071921a2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15 to 15 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 15 | 5 | 5 | [run](https://argusic.com/run/7c46dd91-4083-4306-ac5b-df1deb352ef1) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `gpg binary not installed in container`
- 2 min: `gpg-agent binary not found at hardcoded /usr/bin/gpg-agent path`
- 1 min: `GPG key had no encryption subkey (only SC - Sign/Certify)`
- 1 min: `clear command returns exit code 1 in non-TTY environment, causing emit_pass to fail incorrectly`
- 2 min: `setup_keygroup() grep for 'sec#' does not match non-smartcard keys (shows empty recommended IDs)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
