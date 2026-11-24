# hermes-hudui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/joeynyc/hermes-hudui, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/hermes-hudui

## Pinned environment

- Project commit: `9f6270450e8e86649cb8beb6c59fc43172992483`
- Test commit: `9f6270450e8e86649cb8beb6c59fc43172992483`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4.9 | 3 | 3 | [run](https://argusic.com/run/32bd9786-9f3b-4324-8427-0efe6d306ecb) |
| 2 | pass | 100 | 4 | 2 | 1 | 1 | [run](https://argusic.com/run/d2ab74bd-2324-4a71-81de-b3d7f0e51982) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node.js is v18.19.1 but project requires >=22.12.0`
- 2 min: `No .hermes/ data directory existed, which is expected for a fresh environment`
- `state.db sessions table lacked model_config column needed by sessions collector query`

Attempt 2:

- 2 min: `Node.js 18.19.1 installed but project requires >=22.12.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
