# serverless-domain-manager

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amplify-education/serverless-domain-manager, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/serverless-domain-manager

## Pinned environment

- Project commit: `4bceea12be67d0072ecdbac850484b9acba77574`
- Test commit: `4bceea12be67d0072ecdbac850484b9acba77574`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 2.7 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 2.7 | 1 | 1 | [run](https://argusic.com/run/d6f3863e-1ecd-4479-9fe5-35c97aeeed98) |
| 2 | pass | 100 | 2 | 3.4 | 0 | 0 | [run](https://argusic.com/run/453c0802-3883-42b6-a7ed-77d39cc8ca9e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node v18 present but package engines require node >=20; npm install emitted EBADENGINE warnings`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
