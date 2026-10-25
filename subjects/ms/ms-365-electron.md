# MS-365-Electron

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agam778/MS-365-Electron, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ms-365-electron

## Pinned environment

- Project commit: `d293b8082952387b162549d53243da682dd149eb`
- Test commit: `d293b8082952387b162549d53243da682dd149eb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.5 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.3 | 6.3 | 0 | 0 | [run](https://argusic.com/run/66911224-188b-4b71-a3e3-c7fb49052bad) |
| 2 | fail | 80 | 6.2 | 5.5 | 3 | 3 | [run](https://argusic.com/run/d3a0054f-0aed-4370-88d6-9e6ab0b925f9) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `SUID sandbox helper not configured; electron --version and bare yarn start crash with SIGTRAP`
- 1 min: `GPU process crash: GPU process is not usable without --in-process-gpu flag (fatal SIGILL)`
- `dbus not available in container (non-fatal, bus.cc warnings printed to stderr)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
