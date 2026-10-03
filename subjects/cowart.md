# Cowart

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zhongerxin/Cowart, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/cowart

## Pinned environment

- Project commit: `43fc8882daf2560c7e36fd34a95fe12c251493ac`
- Test commit: `43fc8882daf2560c7e36fd34a95fe12c251493ac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.5 to 15.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 15.5 | 2 | 2 | [run](https://argusic.com/run/ee433713-1683-4ee3-8bb2-e1d265563b93) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `ReferenceError: crypto is not defined in mcp/lib/posthog-analytics.mjs on Node 18 ESM (bare crypto is not a global in Node 18 ES modules)`
- 1 min: `Vite 7 dev server requires Node ^20.19.0||>=22.12.0; Node 18 cannot run npm run dev`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
