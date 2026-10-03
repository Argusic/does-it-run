# infinitunes

**Verdict: runs with mocks.** Argusic Score 87.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rajput-hemant/infinitunes, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/infinitunes

## Pinned environment

- Project commit: `83d0b88a1db72f89a2bc17bfc3f9a4997199561c`
- Test commit: `83d0b88a1db72f89a2bc17bfc3f9a4997199561c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 31.6 to 39.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 31.6 | 4 | 4 | [run](https://argusic.com/run/750e6b73-0745-45ab-8e1e-4676cd087a1d) |
| 2 | pass with mocks | 83.43 | 16 | 39.6 | 7 | 4 | [run](https://argusic.com/run/8beeb8aa-8269-484b-a6d9-4216ce39d7f9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `package.json overrides field contains npm-incompatible alias syntax (npm:types-react@...)`
- 1 min: `npm peer dependency conflict due to React 19 RC version`
- 2 min: `experimental.ppr: true requires canary Next.js, but npm resolved to stable 15.5.25`
- 30 min: `Default JioSaavn API URL (jiosaavn-api-ts.vercel.app) returns DEPLOYMENT_NOT_FOUND`

Attempt 2:

- 1 min: `npm install failed: npm: protocol overrides not supported by npm`
- 1 min: `npm install failed: React 19 RC peer dep conflict with react-hook-form`
- 1 min: `next build failed: experimental.ppr requires canary Next.js (have 15.5.25)`
- 1 min: `next build killed during static page generation (OOM in ~1GB container)`
- `ESLint tailwindcss/enforces-negative-arbitrary-values rule could not resolve tailwindcss`
- `Upstash Redis uses Node.js API not available in Edge Runtime`
- 3 min: `No PostgreSQL for database, no OAuth credentials, no real JioSaavn API key`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
