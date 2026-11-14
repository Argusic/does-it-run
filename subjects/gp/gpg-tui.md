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
- Valid runs: 2; wall time 18.9 to 35.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 35.2 | 1 | 1 | [run](https://argusic.com/run/887c535a-d4c2-4fc8-921d-ddd92aabce2b) |
| 2 | pass | 100 | 18 | 18.9 | 6 | 6 | [run](https://argusic.com/run/63bb60b0-e9f6-45df-a004-fef1e88bf957) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `gpgme set_pinentry_mode(PinentryMode::Ask) failed with 'Not supported (gpg error 60)' because gpgconf hardcodes /usr/bin/gpg but the binary is in a local non-root prefix`

Attempt 2:

- 0.4 min: `rustc/cargo not found`
- 0.5 min: `libgpgme-dev, libgpg-error-dev not installed (no root)`
- 1 min: `pkg-config could not find gpgme, gpg-error, libassuan`
- 5 min: `gpgme_get_dirinfo() returns NULL with extracted GPGME`
- 2 min: `gpg binary not available at runtime`
- `two tests panicked with failed to get homedir`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
