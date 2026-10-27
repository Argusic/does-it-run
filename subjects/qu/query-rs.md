# query.rs

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/huhu/query.rs, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/query-rs

## Pinned environment

- Project commit: `11980451c406a44b4c886645d919a5dca1430bf3`
- Test commit: `11980451c406a44b4c886645d919a5dca1430bf3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.8 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 6.8 | 1 | 1 | [run](https://argusic.com/run/91cf80dd-c807-453e-895a-49b732cf844b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm run build failed with ReferenceError: $state is not defined - @sveltejs/kit@2.70.3 requires Svelte 5 runes but Svelte@4.2.20 was installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
