# cliproxyapi-dashboard

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/itsmylife44/cliproxyapi-dashboard, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cliproxyapi-dashboard

## Pinned environment

- Project commit: `bf6c62956e454b4624b77186415adfd5bfb7d852`
- Test commit: `bf6c62956e454b4624b77186415adfd5bfb7d852`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.4 to 10.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 10.4 | 4 | 4 | [run](https://argusic.com/run/cee6beae-7a30-4b68-bec5-e908f10fc836) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18 (bundled) is too old for Next.js 16 which requires 24+`
- 3 min: `No PostgreSQL server available (no root to apt-install)`
- `MANAGEMENT_API_KEY must be at least 16 characters`
- 1 min: `next start fails with output: standalone config`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
