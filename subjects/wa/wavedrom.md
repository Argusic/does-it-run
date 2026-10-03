# wavedrom

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wavedrom/wavedrom, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/wavedrom

## Pinned environment

- Project commit: `142dd41870bcca7450f55c970d9e3c8070deeb05`
- Test commit: `142dd41870bcca7450f55c970d9e3c8070deeb05`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 3.2 | 1 | 1 | [run](https://argusic.com/run/0c999566-fc46-4a12-a5b5-70ee99165b03) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Container Node v18.19.1 does not satisfy package.json engines requirement >=20; c8@12.0.0 needs >=20.19 and mocha@12.0.0 needs >=20.19`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
