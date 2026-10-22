# openwhyd

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openwhyd/openwhyd, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/openwhyd

## Pinned environment

- Project commit: `9db9783f5bd207d79f683b4a79106ba3e304d811`
- Test commit: `9db9783f5bd207d79f683b4a79106ba3e304d811`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.1 to 13.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 13.1 | 2 | 2 | [run](https://argusic.com/run/8daca00e-30fc-4d7b-a47b-ab6295326a89) |

## What was observed on a clean machine

Attempt 1:

- `gm: not found (GraphicsMagick not installed)`
- `ENOENT: scandir '/work/repo/uAvatarImg'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
