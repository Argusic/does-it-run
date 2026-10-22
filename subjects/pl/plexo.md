# plexo

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/anmolkapil/plexo, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/plexo

## Pinned environment

- Project commit: `5366a8c01c68b53a1d5fcc04cdad41e53444d37f`
- Test commit: `5366a8c01c68b53a1d5fcc04cdad41e53444d37f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 76.7 to 76.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96.67 | 4 | 76.7 | 6 | 5 | [run](https://argusic.com/run/27d78f7e-afad-4509-8372-02086b13b8c2) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `IPv6 disabled in container: 4 E2E tests failed with listen EADDRNOTAVAIL ::1`
- 3 min: `Electron chrome-sandbox SUID not configured in container`
- 8 min: `downloads-page tests: #panel-linux not visible (macOS tab selected for Mac UA)`
- 15 min: `schedule datepicker: calendar popover animation made click unstable`
- 30 min: `moved-file dialog test raced background history re-check (menu lost Show in folder, row label inconsistent)`
- 20 min: `1 hedge timing flake under parallel load (2 KB/s crawl vs 400ms hedge)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
