# pwd.sh

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/drduh/pwd.sh, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/pwd-sh

## Pinned environment

- Project commit: `7a5fd09010a0177dea4cade093b0a07d412ff0ef`
- Test commit: `7a5fd09010a0177dea4cade093b0a07d412ff0ef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.1 to 17.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 17.1 | 4 | 4 | [run](https://argusic.com/run/44de435a-829b-4b1e-8f2a-a41858894cf7) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `GnuPG (gpg binary) not installed in container`
- 2 min: `gpg-agent not found at /usr/bin/gpg-agent (compile-time path)`
- 1 min: `No /usr/share/dict/words - username generation fails`
- `tr: write error: Broken pipe during write (cosmetic)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
