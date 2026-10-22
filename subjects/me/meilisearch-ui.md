# meilisearch-ui

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eyeix/meilisearch-ui, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/meilisearch-ui

## Pinned environment

- Project commit: `ed8a2da42e1209d43e5b190e74617bb5360ce6ad`
- Test commit: `ed8a2da42e1209d43e5b190e74617bb5360ce6ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 21.6 to 23 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 17 | 21.6 | 4 | 4 | [run](https://argusic.com/run/5e216b67-cbfa-4c40-b74d-4e1dae6507b8) |
| 2 | pass with mocks | 92 | 45 | 23 | 8 | 8 | [run](https://argusic.com/run/6b13df8f-c191-4206-b697-a114d4eefd9c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed; required for dependency management`
- 2 min: `pnpm v10 requires pnpm-workspace.yaml for build approval`
- 1 min: `tsc error: 'count' passed as string to i18next t() but expects number`
- 2 min: `tsc error: ECharts v5 dropped itemStyle.normal nesting layer`

Attempt 2:

- 3 min: `Biome lint: node: protocol missing in scripts/post-build.js (3 errors)`
- 4 min: `tsc: Total.tsx passed count:string to i18next (expects number)`
- 12 min: `tsc: ECharts pie used legacy itemStyle.normal (removed in ECharts v5 types)`
- 8 min: `Mock Meilisearch: CORS preflight rejected x-meilisearch-client header`
- 8 min: `Mock Meilisearch: /indexes/{uid}/search returned 404; Documents tab showed 0 hits`
- 3 min: `Mock Meilisearch: /indexes/{uid}/settings returned 404`
- 5 min: `Playwright requires Node >=20 but container has Node 18.19.1`
- 2 min: `vite preview does not honor base placeholder, 302 to /MEILI_UI_REPLACE_BASE_PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
