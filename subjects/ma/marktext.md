# marktext

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/marktext/marktext, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/marktext

## Pinned environment

- Project commit: `0d8dba02bb77efdf33198a3b197bf8fdb42bec79`
- Test commit: `0d8dba02bb77efdf33198a3b197bf8fdb42bec79`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.4 to 15.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 15.4 | 4 | 4 | [run](https://argusic.com/run/83c6d904-e5b8-42b8-a710-76659cced5e2) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed in container`
- 1 min: `Node.js v18.19.1 below required v20.19.0`
- 5 min: `native-keymap build failed: missing X11 -dev headers and pkg-config files (x11.pc, xkbfile.pc, xproto.pc, kbproto.pc)`
- 1 min: `native-keymap linker failed: cannot find -lX11 and -lxkbfile`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
