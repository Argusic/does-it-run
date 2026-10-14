# hippo-memory

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kitfunso/hippo-memory, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hippo-memory

## Pinned environment

- Project commit: `36bb86905d0d94dac43970c9b75779f738ec9d67`
- Test commit: `36bb86905d0d94dac43970c9b75779f738ec9d67`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.1 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 7.1 | 3 | 3 | [run](https://argusic.com/run/66c5ff2f-896c-4555-b24a-eefe9db2ae71) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `System Node is v18.19.1 but the package requires Node >=22.16.0 (engines); npm install and build are unsupported on v18`
- 1 min: `npm run build printed '/bin/sh: 1: Bad substitution'`
- 3 min: `HTTP probes to /v1/memories returned 400 'q is required' and 'content is required'; README does not spell out HTTP field names`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
