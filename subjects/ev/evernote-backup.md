# evernote-backup

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vzhd1701/evernote-backup, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/evernote-backup

## Pinned environment

- Project commit: `749c72666fac050eb0eba1359ed453dc018f17a8`
- Test commit: `749c72666fac050eb0eba1359ed453dc018f17a8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.1 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.1 | 2.1 | 2 | 2 | [run](https://argusic.com/run/5b852b69-5945-48e7-b508-dc03b955bd6d) |

## What was observed on a clean machine

Attempt 1:

- `uv not found in PATH`
- `ty check reports 4 unresolved-import errors for keyring and pycryptodome on Linux`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
