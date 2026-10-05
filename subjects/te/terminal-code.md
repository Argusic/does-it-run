# terminal-code

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zenbu-labs/terminal-code, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/terminal-code

## Pinned environment

- Project commit: `66441668de5fbe142d97ec395ee4f2bd115c5cab`
- Test commit: `66441668de5fbe142d97ec395ee4f2bd115c5cab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.8 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 6.8 | 2 | 2 | [run](https://argusic.com/run/072c6732-adeb-4888-b41e-afad36f20384) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 is too old , vite@8.2.1 requires ^20.19.0 || >=22.12.0`
- 1 min: `unzip not installed; pixel postinstall cannot extract patched electron binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
