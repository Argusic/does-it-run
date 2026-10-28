# codemirror-editor-vue3

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rennzhang/codemirror-editor-vue3, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codemirror-editor-vue3

## Pinned environment

- Project commit: `5636c6f783778ab51deb7b3b9c671d8f93b65eeb`
- Test commit: `5636c6f783778ab51deb7b3b9c671d8f93b65eeb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.6 to 10.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 10.6 | 2 | 2 | [run](https://argusic.com/run/eba6232a-f1a2-4fe1-bf65-588843e82b20) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pnpm not installed and global npm install lacked write permission to /usr/local`
- 1 min: `Nohup-started vite dev server died when its shell exited`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
