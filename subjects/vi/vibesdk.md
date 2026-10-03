# vibesdk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cloudflare/vibesdk, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vibesdk

## Pinned environment

- Project commit: `89c5f3a84c65b86595ed48996aabed68f447c0bd`
- Test commit: `89c5f3a84c65b86595ed48996aabed68f447c0bd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 9.7 to 14.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 9.7 | 1 | 1 | [run](https://argusic.com/run/9cea3378-e47f-4a69-9b0e-1aa5fb8452dd) |
| 2 | pass | 100 | 13 | 14.3 | 6 | 6 | [run](https://argusic.com/run/0cd296a3-a00b-4983-9636-ae29656d6369) |
| 3 | pass | 100 | 12 | 11.1 | 3 | 3 | [run](https://argusic.com/run/d97d3754-b706-4c41-bb75-8fb7c6c192d4) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `System Node v18 lacks node:util.styleText required by rolldown (used by vitest/vite)`

Attempt 2:

- 2 min: `Bun binary not found and unzip not available for the install script`
- 1 min: `Node.js v18.19.1 is below the >=22 requirement, causing rolldown/Vite to fail with 'styleText' SyntaxError`
- 2 min: `Cloudflare Vite plugin tried to establish a remote proxy session, failing with 'You must be logged in'`
- 1 min: `Wrangler tried to build container images from Dockerfile, but Docker is not available`
- 1 min: `Worker FATAL error on startup because CUSTOM_DOMAIN was empty`
- 2 min: `SDK package build failed because dts-bundle-generator was not found`

Attempt 3:

- 2 min: `bun not found in container`
- 2 min: `Node.js v18.19.1 lacks node:util.styleText used by Vitest v3`
- 1 min: `cannot install packages via apt-get (no root) or npm -g (permission denied)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
