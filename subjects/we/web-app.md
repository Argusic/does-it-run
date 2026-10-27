# web-app

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/valhalla/web-app, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/web-app

## Pinned environment

- Project commit: `f7a1dc504347589a1c8e3e4dcfb95b15e555113c`
- Test commit: `f7a1dc504347589a1c8e3e4dcfb95b15e555113c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.3 to 10.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.18 | 10.3 | 1 | 1 | [run](https://argusic.com/run/0eeec667-8139-474c-bb5b-8aecdd468274) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node 18 too old for vite 7 / vitest 4: crypto.hash missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
