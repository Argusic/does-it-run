# FrameScript

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/frame-script/FrameScript, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/framescript

## Pinned environment

- Project commit: `df01b9193b44785d8cbdfd321eb1d7a0735a30c7`
- Test commit: `df01b9193b44785d8cbdfd321eb1d7a0735a30c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 10 | 3 | 3 | [run](https://argusic.com/run/48c9ba11-569b-444b-8113-4c739dd04842) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 is too old for Vite 7 (requires ^20.19.0 or >=22.12.0). Build fails with 'crypto.hash is not a function'.`
- 1 min: `npm install fails because Puppeteer tries to download Chrome but unzip is not installed: 'no zip archiver is available'.`
- 1 min: `Electron binary fails with 'The SUID sandbox helper binary was found, but is not configured correctly' when run without --no-sandbox.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
