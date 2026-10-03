# LinkBreeze

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Manak-hash/LinkBreeze, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/linkbreeze

## Pinned environment

- Project commit: `8335b748e371ae4bdf55d2c765bb190a732f60e5`
- Test commit: `8335b748e371ae4bdf55d2c765bb190a732f60e5`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.8 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8.5 | 9.8 | 2 | 2 | [run](https://argusic.com/run/6788154c-0bb4-4e19-9790-7ad596ac1423) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node.js v18 (system) too old , project requires >=22`
- 3 min: `npm install failed: better-sqlite3 native compilation needs build-essential (gcc/g++/make), not installed and no root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
