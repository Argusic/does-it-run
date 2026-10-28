# notion-electron

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/anechunaev/notion-electron, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/notion-electron

## Pinned environment

- Project commit: `92918ebab0fc90cb935087d93b6bad2972062188`
- Test commit: `92918ebab0fc90cb935087d93b6bad2972062188`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7.2 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 23 | 8.7 | 4 | 4 | [run](https://argusic.com/run/6306dc53-6212-4b5d-ba14-3b8f157369c1) |
| 2 | pass | 100 | 7 | 7.2 | 3 | 3 | [run](https://argusic.com/run/0de2e3c5-7511-41c4-99de-27c46d19ba61) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 installed, project requires v22+`
- `Chrome sandbox SUID not configurable (no root)`
- 3 min: `D-Bus session address parsing failed on ,guid= suffix`
- 1 min: `Unhandled promise rejection from portal Desktop theme query`

Attempt 2:

- 2 min: `Node.js v18 in container, project requires v22+`
- 1 min: `chrome-sandbox SUID helper needs root ownership (container limitation)`
- 3 min: `themeService.queryColorScheme() calls freedesktop portal D-Bus API unavailable in container, crashing app`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
