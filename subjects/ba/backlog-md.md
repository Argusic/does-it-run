# Backlog.md

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MrLesk/Backlog.md, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/backlog-md

## Pinned environment

- Project commit: `c310b7087c3d8d618520bfe4b9918e1c8bc468c4`
- Test commit: `c310b7087c3d8d618520bfe4b9918e1c8bc468c4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 58 to 58 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 58 | 3 | 3 | [run](https://argusic.com/run/c1e7973d-6540-406e-bb23-a4eca794c36e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `bun not installed`
- 2 min: `ssh-keygen not found - test 'preserves commit.gpgSign' requires it`
- 3 min: `Bun YAML parser rejects tab characters - config test 'reads the config key at column 0' failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
