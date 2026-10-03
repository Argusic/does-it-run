# awesome-generative-ai-apps

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Anil-matcha/awesome-generative-ai-apps, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/awesome-generative-ai-apps

## Pinned environment

- Project commit: `8fcaa253fbb81771412f195b215e5b30ae710ee4`
- Test commit: `8fcaa253fbb81771412f195b215e5b30ae710ee4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.1 to 15.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 15.1 | 3 | 3 | [run](https://argusic.com/run/958cd0a8-f24f-473a-9c6b-bcfcda21f2d0) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 too old for Prisma v7 (required >=20.19)`
- 4 min: `No PostgreSQL available - Prisma used @prisma/adapter-pg with pg driver`
- 1 min: `Build failed: import PrismaLibSQL not found in @prisma/adapter-libsql (casing)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
