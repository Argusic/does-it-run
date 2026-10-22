# geek-life

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ajaxray/geek-life, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/geek-life

## Pinned environment

- Project commit: `7e1e10ff3a58f98eb6428152170a682fc5d77d82`
- Test commit: `7e1e10ff3a58f98eb6428152170a682fc5d77d82`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.6 to 3.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 3.6 | 4 | 4 | [run](https://argusic.com/run/efa26453-811b-4343-89f2-a3ab8c3f0194) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go binary not found in PATH (no go compiler)`
- 1 min: `util/util.go line 78: log.Printf does not support error-wrapping directive %w`
- 1 min: `App panics with 'open /dev/tty: no such device or address' when run directly in headless shell`
- `DB_FILE env var or --db-file flag is needed to avoid ~/.geek-life/default.db path which may not exist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
