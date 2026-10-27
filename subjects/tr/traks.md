# traks

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shivamanupadi/traks, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/traks

## Pinned environment

- Project commit: `762280a9a9b1070b81ab67b9216b7586960e9373`
- Test commit: `762280a9a9b1070b81ab67b9216b7586960e9373`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 4 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 8 | 4 | 0 | 0 | [run](https://argusic.com/run/7bc1d4c0-22d9-429b-ad34-231394a2fb43) |
| 2 | pass with mocks | 92 | 18 | 8.7 | 4 | 4 | [run](https://argusic.com/run/33c03c7c-4045-423d-abfe-e3046464a0ce) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js v18.19.1 installed but project requires >=20 (wrangler 4.107.1 requires >=22)`
- 1 min: `Doppler secrets not available (no doppler CLI, no API keys)`
- `Better Auth warns 'BETTER_AUTH_SECRET appears low-entropy'`
- 5 min: `Home API Worker (apps/home/api) cannot start locally , wrangler dev attempts remote connection to R2 bucket traks-releases which requires Cloudflare API credentials`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
