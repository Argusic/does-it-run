# VengeanceUI

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Ashutoshx7/VengeanceUI, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vengeanceui

## Pinned environment

- Project commit: `813d9c192b1f82cb36db3d5af93c2ac7d3285ae4`
- Test commit: `813d9c192b1f82cb36db3d5af93c2ac7d3285ae4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 6.5 to 13.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 12.4 | 0 | 0 | [run](https://argusic.com/run/0e7b4e46-29dc-4c49-ab92-08a2e1440e65) |
| 1 | pass | 100 | 2 | 6.5 | 1 | 1 | [run](https://argusic.com/run/c6bb0cde-a8d4-4f72-a36d-6985d6f9b921) |
| 2 | pass | 100 | 1.5 | 13.4 | 1 | 1 | [run](https://argusic.com/run/95b43a6f-e9a3-4138-9792-a40632bfa9fb) |
| 3 | pass | 100 | 2 | 11 | 3 | 3 | [run](https://argusic.com/run/77fb1399-effc-463d-94eb-a3f8f2d4ef50) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Container has Node.js 18.19.1 but project requires >=20.9.0`

Attempt 2:

- 1 min: `Node.js v18.19.1 was installed but project requires >=20.9.0`

Attempt 3:

- 1 min: `Node.js 18.19.1 is too old for Next.js 16 (requires >=20.9.0)`
- 1 min: `npm install with Node 18 produced broken @tailwindcss/oxide native binding on x64 linux`
- 0.3 min: `Build process ran out of memory (heap OOM)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
