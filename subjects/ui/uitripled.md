# uitripled

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/moumen-soliman/uitripled, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/uitripled

## Pinned environment

- Project commit: `05d18376db775072ed61d0cab8ea184f8f527429`
- Test commit: `05d18376db775072ed61d0cab8ea184f8f527429`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 8.5 to 23 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 23 | 3 | 3 | [run](https://argusic.com/run/3217c6aa-8089-48c8-bd4f-64322d1036d9) |
| 1 | pass | 100 | 7 | 8.5 | 3 | 3 | [run](https://argusic.com/run/642b88b2-c1b4-47b3-9cb8-b0680c47e89b) |
| 2 | pass | 100 | 0.1 | 14 | 2 | 2 | [run](https://argusic.com/run/e09951d6-378f-43bc-9f69-28e98c682ab4) |
| 3 | pass | 100 | 1.5 | 16.4 | 2 | 2 | [run](https://argusic.com/run/3d24e6ea-2fa7-44f8-9644-40de7077b75f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18.19.1 too old for Next.js 16 (requires >=20.9.0)`
- 2 min: `pnpm not found in container`
- 10 min: `Turbopack dev mode fails with 'Too many open files (os error 24)' despite ulimit -n 524288`

Attempt 1:

- 2 min: `Node.js 18 is installed but Next.js 16 requires >=20.9.0`
- 1 min: `pnpm 9.15.4 not found in path`
- `/hall-of-fame page fetch to GitHub API fails without credentials`

Attempt 2:

- 2 min: `Node.js 18.19.1 too old for Next.js 16 (requires >=20.9.0)`
- 1 min: `6 packages missing eslint.config.mjs files causing lint failures`

Attempt 3:

- 1 min: `Node.js 18.19.1 is incompatible with Next.js 16 which requires >=20.9.0`
- 2 min: `Dev server hangs on subsequent requests after first response`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
