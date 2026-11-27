# squad

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/github/squad, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/4abc378f-0ae4-4826-8248-cfe8815d067d

## Pinned environment

- Project commit: `7b731ec97f35346bdc4fa87c3edaf16b808fc0ae`
- Test commit: `7b731ec97f35346bdc4fa87c3edaf16b808fc0ae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 41.9 to 41.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 41.9 | 3 | 3 | [run](https://argusic.com/run/4abc378f-0ae4-4826-8248-cfe8815d067d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 , project requires >=22.5.0`
- `98 tests fail: spawnSync gh ENOENT , GitHub CLI not installed, tests need gh aw compile`
- `84 tests fail: vscode-jsonrpc exports issue in isolated temp dirs (ERR_PACKAGE_PATH_NOT_EXPORTED)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
