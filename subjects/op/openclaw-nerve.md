# openclaw-nerve

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/daggerhashimoto/openclaw-nerve, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openclaw-nerve

## Pinned environment

- Project commit: `312e27333e14f841b95bf4f2b205a856b4a4c370`
- Test commit: `312e27333e14f841b95bf4f2b205a856b4a4c370`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 13 | 1 | 1 | [run](https://argusic.com/run/679ff0b8-cc28-48b1-bb28-c40d45a461dd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18.19.1 is below required Node 22+`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
