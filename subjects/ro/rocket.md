# rocket

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/modernweb-dev/rocket, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/rocket

## Pinned environment

- Project commit: `c4a9515064513883f08b1f05ac4624d37b8af639`
- Test commit: `c4a9515064513883f08b1f05ac4624d37b8af639`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.5 to 12.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 12.5 | 3 | 3 | [run](https://argusic.com/run/1977c2ca-6c9d-4d00-8fb4-18c13dffb3dd) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Node 18 present but package requires Node >=22; npm ci could still install but vite engine warning`
- 6 min: `Browser tests failed: no Chrome executable found, then bundled Chromium 149 failed with 'No usable sandbox'`
- 14 min: `Dev server started but returned 404 for every page: markdownHook registered via relative path resolved against npx cache dir, crashing page scan; plugin also treated curl's Accept: */* as non-page`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
