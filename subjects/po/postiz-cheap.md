# postiz-cheap

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SamurAIGPT/postiz-cheap, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/postiz-cheap

## Pinned environment

- Project commit: `2c42b7a621d5eb590950b86c121ea31106c45f4e`
- Test commit: `2c42b7a621d5eb590950b86c121ea31106c45f4e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 7.2 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 8.2 | 1 | 1 | [run](https://argusic.com/run/0db4fd52-bfc1-40e1-9d63-db99b6379c88) |
| 2 | pass with mocks | 92 | 8 | 7.2 | 4 | 4 | [run](https://argusic.com/run/569e22ab-7dc3-4df5-a98e-3024e3ea87ba) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 too old for Next.js 16 (needs >=20.9.0) and Prisma 7 (needs >=20.19)`

Attempt 2:

- 2 min: `Node.js 18 is too old (requires Node ^20.19||^22.12||>=24.0). npm install failed on Prisma preinstall check.`
- 3 min: `POST /api/posts route called .toLowerCase() on objects from body.platforms array, crashing with 'plat.toLowerCase is not a function'`
- 1 min: `PostgreSQL not available in container , prisma.scheduledPost.findMany throws connection refused`
- `npm warns about deprecated uuid and engine mismatch for eslint-visitor-keys`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
