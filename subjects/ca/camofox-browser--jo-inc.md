# camofox-browser

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jo-inc/camofox-browser, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/9bfec9b8-f14f-46a9-b40a-66ce69712532

## Pinned environment

- Project commit: `389c996ae3c7d42e539295a336ee6f975847f066`
- Test commit: `389c996ae3c7d42e539295a336ee6f975847f066`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.1 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 4.1 | 0 | 0 | [run](https://argusic.com/run/9bfec9b8-f14f-46a9-b40a-66ce69712532) |
| 2 | pass | 93.33 | 12 | 12.6 | 3 | 2 | [run](https://argusic.com/run/ba386a66-6a8e-4e68-8e30-e97ad8ed67d8) |

## What was observed on a clean machine

Attempt 2:

- 4 min: `Node.js version mismatch: package.json requires >=22, system had 18.19`
- 2 min: `npm install failed on openclaw preinstall requiring Node >=24`
- `1 pre-existing test failure: tabLifecycleContract popup tab count expects >=2 but got 1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
