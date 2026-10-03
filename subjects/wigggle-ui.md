# Wigggle UI

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wigggle-ui/ui, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/wigggle-ui

## Pinned environment

- Project commit: `b0936d8779a3a121dcd4ccbe2ac8f549486c45c6`
- Test commit: `b0936d8779a3a121dcd4ccbe2ac8f549486c45c6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 4; wall time 6 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 8.9 | 1 | 1 | [run](https://argusic.com/run/6166152b-5122-40a4-beb1-6d5bc6cfe629) |
| 1 | fail | 80 | 2 | 9.3 | 1 | 1 | [run](https://argusic.com/run/26f380b6-9ccd-47a3-95be-2ef2806d00a9) |
| 2 | pass | 100 | 8 | 6.7 | 2 | 2 | [run](https://argusic.com/run/1894e552-cfbb-4b31-bf34-84e0e8e91c49) |
| 3 | pass | 100 | 2 | 6 | 1 | 1 | [run](https://argusic.com/run/98f95d48-84c6-4128-a955-020bcd916bd1) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js 18.19.1 is too old for Next.js 16 (requires >=20.9.0) - npm install succeeded but next build would fail without upgrading`

Attempt 1:

- 2 min: `Node.js 18.19.1 is too old for Next.js 16 (requires >=20.9.0). 'npm run build' failed with 'You are using Node.js 18.19.1. For Next.js, Node.js version >=20.9.0 is required.'`

Attempt 2:

- 2 min: `Node.js 18.19.1 is insufficient for Next.js 16 which requires >=20.9.0`
- 1 min: `Missing required environment variables: OPEN_PANEL_CLIENT_ID (used with non-null assertion) and NEXT_PUBLIC_WANDRY_REGISTRY_TOKEN`

Attempt 3:

- 2 min: `Node.js 18.19.1 too old for Next.js 16 (requires >=20.9.0)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
