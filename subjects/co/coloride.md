# coloride

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Color-IDE/coloride, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/coloride

## Pinned environment

- Project commit: `5c7eab5b265e63f0e142070ff95807631ce23819`
- Test commit: `5c7eab5b265e63f0e142070ff95807631ce23819`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 7.5 | 5 | 5 | [run](https://argusic.com/run/5df136c4-e5df-4445-aa98-145c5e95df3f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Host Node.js was v18 instead of required v22; corepack absent`
- `Agent runtime bundle not built , bundled_runtime_script() returned None`
- `Electron sandbox in container: SUID sandbox helper not owned by root`
- `cross-env not on PATH with raw shell launch`
- `/bin/zsh not installed , one test depends on zsh subprocess`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
