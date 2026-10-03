# presenterm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mfontanini/presenterm, licensed BSD-2-Clause, written in Rust.

Evidence and recordings: https://argusic.com/subject/presenterm

## Pinned environment

- Project commit: `5f8add11a24af9d257fd18da48c8004dd9c516f8`
- Test commit: `5f8add11a24af9d257fd18da48c8004dd9c516f8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 6.6 | 2 | 2 | [run](https://argusic.com/run/2188946c-efb3-4032-89e2-9708d14c723e) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Interactive TUI commands (--list-themes, --validate-overflows, present) fail in headless environment with 'No such device or address (os error 6)' from kitty image protocol requiring a real TTY`
- `PDF export requires weasyprint (Python library) which is not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
