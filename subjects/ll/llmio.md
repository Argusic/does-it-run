# llmio

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/atopos31/llmio, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/llmio

## Pinned environment

- Project commit: `3919f3385eb372911d8b91e8b025b26d9473491e`
- Test commit: `3919f3385eb372911d8b91e8b025b26d9473491e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.3 to 16.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10.2 | 16.3 | 5 | 5 | [run](https://argusic.com/run/242a78db-bb8c-43be-af52-386a8d413336) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Go binary not found in PATH`
- 0.5 min: `pnpm not found`
- 0.3 min: `Go build failed: pattern webui/dist: no matching files found`
- 4 min: `pnpm ERR_PNPM_IGNORED_BUILDS for @swc/core, esbuild, @tailwindcss/oxide`
- 1 min: `npm install failed due to peer dependency conflicts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
