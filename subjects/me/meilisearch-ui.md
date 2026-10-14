# meilisearch-ui

**Verdict: not yet verified.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eyeix/meilisearch-ui, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/meilisearch-ui

## Pinned environment

- Project commit: `ed8a2da42e1209d43e5b190e74617bb5360ce6ad`
- Test commit: `ed8a2da42e1209d43e5b190e74617bb5360ce6ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 1; wall time 21.6 to 21.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 17 | 21.6 | 4 | 4 | [run](https://argusic.com/run/5e216b67-cbfa-4c40-b74d-4e1dae6507b8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed; required for dependency management`
- 2 min: `pnpm v10 requires pnpm-workspace.yaml for build approval`
- 1 min: `tsc error: 'count' passed as string to i18next t() but expects number`
- 2 min: `tsc error: ECharts v5 dropped itemStyle.normal nesting layer`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
