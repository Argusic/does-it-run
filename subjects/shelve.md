# shelve

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HugoRCD/shelve, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/shelve

## Pinned environment

- Project commit: `377fdc8bd3b76f33faab111fd1747176c7018f6d`
- Test commit: `377fdc8bd3b76f33faab111fd1747176c7018f6d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.8 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 13.8 | 4 | 4 | [run](https://argusic.com/run/0329363f-0a41-4981-b6ae-979bfa00b088) |
| 2 | pass | 100 | 3.5 | 11.8 | 3 | 3 | [run](https://argusic.com/run/85308900-9589-4e69-873c-01973dc5fc94) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node.js v18 is too old for pnpm 11; pnpm 11 requires Node.js >=22.13`
- 1 min: `Missing required env vars NUXT_SESSION_PASSWORD and NUXT_PRIVATE_ENCRYPTION_KEY blocked postinstall`
- 1 min: `@shelve/lp Nuxt build ran out of memory (JavaScript heap OOM)`
- `Vault .output/server directory was empty after cascading failure from initial full build`

Attempt 2:

- 2 min: `Node.js v18.19.1 too old for pnpm 11.1.3 (needs >=22.13)`
- 1 min: `pnpm not available initially, npm install -g failed due to permissions`
- 0.5 min: `Postinstall env validation failed due to missing NUXT_SESSION_PASSWORD and NUXT_PRIVATE_ENCRYPTION_KEY`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
