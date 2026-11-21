# arkit

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dyatko/arkit, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/arkit

## Pinned environment

- Project commit: `fdfd8b30769ca853c70984c6025da273803a2b46`
- Test commit: `fdfd8b30769ca853c70984c6025da273803a2b46`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 4.8 to 27.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 27 | 27.3 | 2 | 2 | [run](https://argusic.com/run/57949b6d-8b99-450c-8fbe-356e8f6385b0) |
| 2 | pass | 100 | 25 | 4.8 | 3 | 3 | [run](https://argusic.com/run/4fa162c8-f51b-4a18-9eee-7fccd38f2450) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `node-plantuml postinstall script fails: spawn java ENOENT`
- 1 min: `Node v18.19.1 but package requires >=20; engine warnings`

Attempt 2:

- 5 min: `Node.js v18 is below the required >=20.0.0`
- 8 min: `Java JRE not installed (needed by node-plantuml for SVG/PNG conversion)`
- 3 min: `node-plantuml postinstall script get-vizjs.js failed because java was not in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
