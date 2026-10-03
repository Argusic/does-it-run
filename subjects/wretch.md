# wretch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elbywan/wretch, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/wretch

## Pinned environment

- Project commit: `32d5f68badf7e8f103b734febe680968c6e0f97f`
- Test commit: `32d5f68badf7e8f103b734febe680968c6e0f97f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.7 to 5.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 5.7 | 4 | 4 | [run](https://argusic.com/run/402617e7-b6d8-4055-8f67-fbaaea67fb5a) |

## What was observed on a clean machine

Attempt 1:

- 6.5 min: `Node.js v18 installed but project requires >=22, preventing build`
- 3 min: `Playwright browsers (chromium_headless_shell, firefox) not found in cache`
- 0.5 min: `Deno --sloppy-imports flag renamed to --unstable-sloppy-imports in Deno 2.x`
- 0.1 min: `Deno lockfile v5 unsupported by Deno 2.2.7`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
