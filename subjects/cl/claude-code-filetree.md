# claude-code-filetree

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/data-goblin/claude-code-filetree, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/claude-code-filetree

## Pinned environment

- Project commit: `91080e6731e84e7b3d79925f32afefdf558c72c1`
- Test commit: `91080e6731e84e7b3d79925f32afefdf558c72c1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 5.1 to 14.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 14 | 14.4 | 1 | 1 | [run](https://argusic.com/run/2a036e38-a441-48fa-a927-d4ca6af82fb2) |
| 2 | pass | 100 | 0.2 | 5.1 | 0 | 0 | [run](https://argusic.com/run/bc67d64d-89c1-4032-9701-93a6a7191f0f) |

## What was observed on a clean machine

Attempt 1:

- 9 min: `System package 'file' missing (rootless Ubuntu image with no /usr/bin/file)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
