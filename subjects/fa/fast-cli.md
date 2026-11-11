# fast-cli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sindresorhus/fast-cli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/fast-cli

## Pinned environment

- Project commit: `378e3ef9b7b15433d0fae8b67db4ab9c6d1de352`
- Test commit: `378e3ef9b7b15433d0fae8b67db4ab9c6d1de352`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.8 to 55.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.6 | 55.8 | 2 | 2 | [run](https://argusic.com/run/9fac3438-c555-4244-b97b-ba41bbeb7bc4) |
| 2 | pass | 100 | 1 | 14.8 | 2 | 2 | [run](https://argusic.com/run/aab5ad4b-6a4b-48a6-8084-8734133a5a45) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 does not meet >=20 requirement`
- 10 min: `Upload tests (upload flag, json upload output) timeout at 90s with Protocol error (Runtime.callFunctionOn): Target closed`

Attempt 2:

- 0.5 min: `Node.js v18.19.1 installed, but project requires >=20. The tsc build and runtime crash with SyntaxError on /v regex flag`
- `Tests time out when running together via npm test (6 real Chrome browsers competing for resources)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
