# llm-wiki-compiler

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/atomicstrata/llm-wiki-compiler, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/llm-wiki-compiler

## Pinned environment

- Project commit: `3fa9f37325f9e2963738964d8c1bb38d7e8f09ac`
- Test commit: `3fa9f37325f9e2963738964d8c1bb38d7e8f09ac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 81.4 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/2f4398ac-bbce-49da-aa56-b1ea8fdad998) |
| 2 | pass | 100 | 2 | 81.4 | 3 | 3 | [run](https://argusic.com/run/05ca8850-fa46-4f00-9588-25764a9f74a6) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Build OOM with default Node options`
- 1 min: `Node.js >=24 required, system has v18.19.1`
- 5 min: `1300/1303 test files pass; 3 failures due to container limitations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
