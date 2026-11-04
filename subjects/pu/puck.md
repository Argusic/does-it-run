# puck

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/puckeditor/puck, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/puck

## Pinned environment

- Project commit: `449f42df3abd2193ad3e740287dc0bcf044b2bfb`
- Test commit: `449f42df3abd2193ad3e740287dc0bcf044b2bfb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7 to 14.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.1 | 14.9 | 0 | 0 | [run](https://argusic.com/run/4f738c4b-1754-432e-b209-229d2ebba4b1) |
| 2 | pass | 100 | 8 | 7 | 5 | 5 | [run](https://argusic.com/run/83c8685d-886a-4aeb-a4f2-80ad9446a0d2) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pnpm not found in PATH`
- 2 min: `Node.js v18.19.1 , project requires >=24`
- 1 min: `npm install -g pnpm failed EACCES on /usr/local/lib`
- 1 min: `Puppeteer: No usable sandbox in container`
- `Smoke test process.stdout.moveCursor not a function (non-TTY terminal)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
