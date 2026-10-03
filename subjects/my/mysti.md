# Mysti

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DeepMyst/Mysti, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mysti

## Pinned environment

- Project commit: `6d709229b5199f6769fb3cf763e5122dcc43c079`
- Test commit: `6d709229b5199f6769fb3cf763e5122dcc43c079`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 4.7 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.7 | 1 | 1 | [run](https://argusic.com/run/c7fabc6c-f7ae-4a14-9c6e-ec12446d5ec2) |
| 2 | pass with mocks | 92 | 5 | 5 | 1 | 1 | [run](https://argusic.com/run/bc02d75c-a7a0-4c90-930c-98e6a81defce) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `vitest v4 (^4.0.18) requires Node >=20 but container has Node 18.19.1: ERR_REQUIRE_ESM startup failure`

Attempt 2:

- 2 min: `vitest 4.x requires Node 20+ (container has Node 18) , ERR_REQUIRE_ESM from vite/vitest`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
