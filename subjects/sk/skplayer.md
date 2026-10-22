# skPlayer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/feilongcheng/skPlayer, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/skplayer

## Pinned environment

- Project commit: `d27142bf3b0b0447b0b5dd413efc39e7aee62ad5`
- Test commit: `d27142bf3b0b0447b0b5dd413efc39e7aee62ad5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.8 to 11.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 11.8 | 4 | 4 | [run](https://argusic.com/run/791dd489-6005-4a62-a7e3-c6ff3e78eec5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm install failed: node-sass node-gyp could not find 'python' (only python3 present) and its dependency sass-loader pinned node-sass@4`
- 5 min: `container-wide /usr/bin/node (Debian-patched Node 18.19.1) reports NODE_MODULE_VERSION 109 while its headers say 108, so node-sass prebuilds never dlopen`
- 1 min: `node-sass 4.14.1 rejects ABI 108 as 'Unsupported runtime' because its allow-list stops at Node 14`
- 1 min: `webpack dev/default build failed when WC command ran outside official Node PATH; also dev script flags (--process, --progress) unsupported by webpack-dev-server 2 in this container setup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
