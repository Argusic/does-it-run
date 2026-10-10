# electrodb

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tywalch/electrodb, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/electrodb

## Pinned environment

- Project commit: `0ceff2015d85eae80b8eb951af7a706540b42fa2`
- Test commit: `0ceff2015d85eae80b8eb951af7a706540b42fa2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 61.4 to 61.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 21 | 61.4 | 3 | 3 | [run](https://argusic.com/run/edb8a27f-83ea-4393-a3c4-7f79cb34b62c) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Full test suite requires Docker-based amazon/dynamodb-local (project test.sh) and Java; neither available rootless in container`
- 5 min: `test/definitions JSON table fixtures were DynamoDB-invalid (GSIs with up to 7 key members; DynamoDB allows max 2), so table provisioning failed`
- 1 min: `25 test failures remain when full connected suite runs against fakecloud (of 5401): all are emulator-internal differences (attribute ordering in returned items, set/list ADD ordering, validation/transaction error message wording, UPDATED_NE`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
