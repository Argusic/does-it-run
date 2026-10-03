# kordoc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chrisryugj/kordoc, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/kordoc

## Pinned environment

- Project commit: `dd4a08b77784abd0a2f1c37e7a8141b1cc522525`
- Test commit: `dd4a08b77784abd0a2f1c37e7a8141b1cc522525`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 13.4 to 27.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 13.4 | 1 | 1 | [run](https://argusic.com/run/71313e96-fa5e-4c37-93e6-ebdc370aba5a) |
| 2 | pass | 100 | 0.6 | 27.8 | 1 | 1 | [run](https://argusic.com/run/ce5c72a5-91d0-4a3b-9f28-ca773af034fc) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `sharp@^0.35.0 requires Node >=20.9.0, but container has Node 18.19.1 , builds succeeded but PNG/raster tests and CLI PNG format would fail at runtime`

Attempt 2:

- 10 min: `sharp 0.35.x requires Node >=20.9.0 but container has Node 18.19.1 , 14 tests fail at load time`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
