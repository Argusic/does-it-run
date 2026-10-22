# simple-todo-c

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Efeckc17/simple-todo-c, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/simple-todo-c

## Pinned environment

- Project commit: `bcdf3d5fcebb8c0b445edb791d54511194c1b6ca`
- Test commit: `bcdf3d5fcebb8c0b445edb791d54511194c1b6ca`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.1 to 23.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 23.1 | 4 | 4 | [run](https://argusic.com/run/f319e8df-abde-4d64-8157-9532e168b0c8) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No mingw-w64 cross-compiler pre-installed in container`
- 3 min: `wine binary could not find NLS locale files (hardcoded /usr/share/wine/nls)`
- 5 min: `Wine user32.dll requires zlib1.dll which is missing from the libwine package`
- `OLE/RPCSS service errors at runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
