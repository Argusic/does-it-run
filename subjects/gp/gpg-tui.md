# gpg-tui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/orhun/gpg-tui, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/gpg-tui

## Pinned environment

- Project commit: `9fb341e0a1ee00a0d903e4810083bed777108448`
- Test commit: `9fb341e0a1ee00a0d903e4810083bed777108448`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.2 to 35.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 35.2 | 1 | 1 | [run](https://argusic.com/run/887c535a-d4c2-4fc8-921d-ddd92aabce2b) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `gpgme set_pinentry_mode(PinentryMode::Ask) failed with 'Not supported (gpg error 60)' because gpgconf hardcodes /usr/bin/gpg but the binary is in a local non-root prefix`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
