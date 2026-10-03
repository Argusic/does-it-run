# Ackee

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/electerious/Ackee, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ackee

## Pinned environment

- Project commit: `c9fe8f889e4f3264e39cdf2343e12b465aa29446`
- Test commit: `c9fe8f889e4f3264e39cdf2343e12b465aa29446`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 4 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 10.8 | 2 | 2 | [run](https://argusic.com/run/bcb0030f-094a-4183-b4c6-2020aa8d30c7) |
| 2 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/9a1799d9-fbf2-447c-935e-29a47dbcf539) |
| 3 | pass | 100 | 2 | 4 | 2 | 2 | [run](https://argusic.com/run/035dfa99-6c43-482f-947a-7ad23c1287fd) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Node.js v18 found, project requires >=24`
- 1 min: `npm install-scripts policy blocked mongodb-memory-server postinstall`

Attempt 3:

- 1 min: `Node.js v18.19.1 is too old; project requires >=24`
- 1 min: `npm test lint step failed due to Prettier formatting of package.json`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
