# mande

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/posva/mande, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mande

## Pinned environment

- Project commit: `5b4ed14cd002670fa50d0c813d4ff7556b1d1337`
- Test commit: `5b4ed14cd002670fa50d0c813d4ff7556b1d1337`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 4.2 | 5 | 5 | [run](https://argusic.com/run/2cee5c24-e81f-42d5-8bde-54f970ff3a7b) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found on PATH`
- 1 min: `Node.js v18.19.1 too old for rolldown (needs ^20.19.0 || >=22.12.0)`
- 0.5 min: `@rolldown/binding-linux-x64-gnu optional dependency not installed (pnpm skips optional deps by default)`
- 0.5 min: `unrun peer dependency of tsdown not installed`
- 0.3 min: `nuxt-module playground tsconfig.json extends ./.nuxt/tsconfig.json which does not exist without nuxi prepare`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
