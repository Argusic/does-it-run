# caddy-proxy-manager

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fuomag9/caddy-proxy-manager, licensed NOASSERTION, written in TypeScript.

Evidence and recordings: https://argusic.com/run/ebc0903b-5ffb-48e1-b538-667d3821006d

## Pinned environment

- Project commit: `927144e6c5b1ccce8ac8974638f05fd5bdfe496f`
- Test commit: `927144e6c5b1ccce8ac8974638f05fd5bdfe496f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.4 to 24.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 24.4 | 3 | 3 | [run](https://argusic.com/run/ebc0903b-5ffb-48e1-b538-667d3821006d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 is too old for vitest 5.x / rolldown 1.x (needs node:util.styleText)`
- 2 min: `maplibre-worker-staging test failed: maplibre-gl v6.16.0 inlines all worker chunks into one file, test asserted deps contained 'maplibre-gl-shared.mjs'`
- 3 min: `@tailwindcss/oxide native optional dependency not resolved by npm (common npm optional-deps issue)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
