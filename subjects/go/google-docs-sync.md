# google-docs-sync

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cedricdelpoux/google-docs-sync, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/google-docs-sync

## Pinned environment

- Project commit: `efe722c0f663f1b33a8d6ec70e350ec3637de73d`
- Test commit: `efe722c0f663f1b33a8d6ec70e350ec3637de73d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.2 | 2 | 2 | [run](https://argusic.com/run/38f010ee-2678-4e8b-a386-bf79efdf4a17) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18 on system path, but project requires >=22.12`
- 1 min: `Missing @rolldown/binding-linux-x64-gnu optional dependency (npm did not install it during npm install)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
