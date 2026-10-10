# jev

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/feder-cr/jev, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/jev

## Pinned environment

- Project commit: `eb74cf78e5377e85fcaa76f6ebc9f82e8b517250`
- Test commit: `eb74cf78e5377e85fcaa76f6ebc9f82e8b517250`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 6.5 | 2 | 2 | [run](https://argusic.com/run/d77612b0-cc66-4264-abca-48e941dfe038) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `uv was not installed in the container`
- 4 min: `README quickstart points to a jevos release asset (jevos-q4_k_m.gguf) that returns 404 on GitHub`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
