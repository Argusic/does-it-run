# pruvious

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pruvious/pruvious, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pruvious

## Pinned environment

- Project commit: `7a3df34236e2c804df21df7bb292e1112aaf242c`
- Test commit: `7a3df34236e2c804df21df7bb292e1112aaf242c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.8 to 12.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 12.8 | 2 | 2 | [run](https://argusic.com/run/721300e6-360e-497a-9a25-488a2aaeae50) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `pnpm build failed: nuxt-module-build could not resolve extends ./.nuxt/tsconfig.json because .nuxt types were not generated (container had no pnpm and only Node 18; repo requires node >=20 and pnpm 11.1.3)`
- 4 min: `pnpm dev playground app served HTTP 404 on / because app.vue renders <NuxtPage /> with no pages/ directory`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
