# chat-demo

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deepseek-ai/chat-demo, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/chat-demo

## Pinned environment

- Project commit: `5d5dd754ebc1948e977ddb880a9eb5aa25f37b4c`
- Test commit: `5d5dd754ebc1948e977ddb880a9eb5aa25f37b4c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 1.6 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 1.6 | 2 | 2 | [run](https://argusic.com/run/9e763490-88cc-4625-b436-a13e0482db20) |
| 2 | fail | 80 | 3 | 4.2 | 2 | 2 | [run](https://argusic.com/run/4508bdad-218b-4ed1-b8ed-5e976d74fc7a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 bundled in container, but Rspack requires Node.js 20.19+ or 22.12+`
- 1 min: `pnpm not pre-installed; npm install -g pnpm failed due to EACCES on /usr/local`

Attempt 2:

- 1 min: `Node.js v18.19.1 too old; Rspack 2.0.2 requires Node.js 20.19+ or 22.12+`
- 1 min: `pnpm not on PATH after global npm install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
