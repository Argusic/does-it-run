# pagescms

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hunvreus/pagescms, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pagescms

## Pinned environment

- Project commit: `6f4e860a35d934406580287e7042e5e111e207a1`
- Test commit: `6f4e860a35d934406580287e7042e5e111e207a1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.4 to 13.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 13.4 | 5 | 5 | [run](https://argusic.com/run/6000a086-2c14-4dcd-8671-255f04e01c6f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18 is too old for Next.js 16 (requires >=20.9.0)`
- 1 min: `Missing native binding @tailwindcss/oxide-linux-x64-gnu after npm install on Node 18 (known npm optional-dependency bug)`
- 3 min: `PostgreSQL not installed in container; no root/sudo to apt-get install`
- 1 min: `PostgreSQL could not bind to /var/run/postgresql (no such directory) and IPv6 ::1`
- 1 min: `npm peer dependency conflict: @base-ui/react requires date-fns^4.0.0 but project has date-fns@3.6.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
