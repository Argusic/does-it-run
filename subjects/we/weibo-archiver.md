# Weibo-archiver

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Chilfish/Weibo-archiver, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/weibo-archiver

## Pinned environment

- Project commit: `2416eafa798ddabc2b4ea66357e3b8e19f3b13ba`
- Test commit: `2416eafa798ddabc2b4ea66357e3b8e19f3b13ba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 4.4 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 18 | 4.4 | 5 | 5 | [run](https://argusic.com/run/f5e694b0-ec81-4969-9c44-86087f29eb9a) |
| 2 | fail | 80 | 6 | 9.7 | 4 | 4 | [run](https://argusic.com/run/f51de581-689b-4fd1-8275-6c257162e69b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js version 18.19.1 < required 20.9.0`
- 1 min: `pnpm version 9.2.0 < required 9.4.0`
- 1 min: `pnpm 11.1.2 requires Node >=22.13`
- 2 min: `rolldown binding-linux-x64-gnu optional dependency missing`
- 1 min: `Go binary not found in PATH`

Attempt 2:

- 2 min: `Node.js v18 too old, project requires >= 20.9.0`
- 1 min: `pnpm not installed, npm install -g failed due to EACCES on /usr/local/lib`
- 2 min: `pnpm 11.1.2 requires Node >= v22.13 but Node v20.18.3 was used after first upgrade`
- 1 min: `rm -rf rejected by sandbox; cannot delete node_modules directly`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
