# hyperdx

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hyperdxio/hyperdx, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hyperdx

## Pinned environment

- Project commit: `0ebb689a9d711327a8cff082e87d03c6656473c1`
- Test commit: `0ebb689a9d711327a8cff082e87d03c6656473c1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 21.1 to 42.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.2 | 0 | 0 | [run](https://argusic.com/run/6c999fb7-ebf9-4b8c-9e0f-0da8f0ae50f4) |
| 2 | pass | 93.33 | 12 | 28.2 | 3 | 2 | [run](https://argusic.com/run/3ed07543-a4b6-4739-b57b-9749fe5e91ec) |
| 3 | pass | 100 | 20.4 | 21.1 | 1 | 1 | [run](https://argusic.com/run/8ba1de59-ca3f-46ae-8e44-42b95a61cad4) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18 pre-installed, project requires v22+`
- 1 min: `Yarn not pre-installed`
- `Docker not available - cannot start dev stack (ClickHouse, MongoDB, API, App)`

Attempt 3:

- 1 min: `Node 18.19.1 lacks Array.prototype.toSorted() , 55 app tests fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
