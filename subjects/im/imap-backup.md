# imap-backup

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/joeyates/imap-backup, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/imap-backup

## Pinned environment

- Project commit: `9431475e561b1aee567d0b61d8efb52c9e663f13`
- Test commit: `9431475e561b1aee567d0b61d8efb52c9e663f13`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 6.9 to 48 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 48 | 0 | 0 | [run](https://argusic.com/run/5aa21869-64e2-47f5-95e2-fe6f0c06bf3b) |
| 2 | pass with mocks | 92 | 3 | 6.9 | 2 | 2 | [run](https://argusic.com/run/0317e8f6-b367-4a4e-a48e-9c4341dce7a8) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Ruby not installed in container , no ruby, gem, or bundle found in PATH`
- 1 min: `fiddle gem (C extension) failed to build: missing libffi.so symlink for linking`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
