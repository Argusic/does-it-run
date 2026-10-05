# TidGi-Desktop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tiddly-gittly/TidGi-Desktop, licensed MPL-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tidgi-desktop

## Pinned environment

- Project commit: `b4540b409b6d3d308afb62579ba2c8966b837e51`
- Test commit: `b4540b409b6d3d308afb62579ba2c8966b837e51`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 7 | 3 | 3 | [run](https://argusic.com/run/08e64f52-3aa1-4c55-b51a-441fa3c4f1c9) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node v18.19.1 is too old , pnpm 11.17.0 requires >=22.13`
- 2 min: `pnpm not found in PATH; npm install -g failed with EACCES writing to /usr/local`
- 1 min: `Git submodule template/wiki not initialized`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
