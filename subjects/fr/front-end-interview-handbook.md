# front-end-interview-handbook

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yangshun/front-end-interview-handbook, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/front-end-interview-handbook

## Pinned environment

- Project commit: `75ee62afc63bb9b48be160b0710bfcba6ab01a75`
- Test commit: `75ee62afc63bb9b48be160b0710bfcba6ab01a75`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10 | 4 | 4 | [run](https://argusic.com/run/3a74a1e6-2c2a-43ae-85ff-afcd3976232c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `global npm install of pnpm@10.28.1 failed: EACCES on /usr/local (npm prefix not writable, no root)`
- 3 min: `pnpm install failed in prepare script: vite-plus imports node:util styleText, which does not exist in bundled Node v18.19.1 (SyntaxError)`
- 1 min: `pnpm run build / pnpm run website#build reported ERR_PNPM_NO_SCRIPT Missing script: build (scripts live under vp run tasks, not package.json)`
- 2 min: `npx serve -l 4000 exited silently (no process, HTTP 000)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
