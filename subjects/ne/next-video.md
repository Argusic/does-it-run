# next-video

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/muxinc/next-video, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/next-video

## Pinned environment

- Project commit: `fefd0ff0a500e5c8cb8510f33d4d01587ea9ac71`
- Test commit: `fefd0ff0a500e5c8cb8510f33d4d01587ea9ac71`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.8 to 28.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.3 | 3.8 | 0 | 0 | [run](https://argusic.com/run/0bec0ee9-4c45-4870-8282-ea984f5305e9) |
| 2 | pass | 100 | 1 | 28.9 | 2 | 2 | [run](https://argusic.com/run/e6294fa0-eaf4-4191-8dd6-3ed192978f93) |

## What was observed on a clean machine

Attempt 2:

- 45 min: `Flaky test failure in create-demo-page.test.ts: 'Unable to deserialize cloned data due to invalid or unsupported version.' , Node 18 test runner bug with tsx loader when running multiple test files concurrently in a single process`
- 30 min: `Flaky test failure in updateNextConfig 'should inject withNextVideo inside existing plugin wrappers' , race condition from test file temp directory cleanup when test suites run concurrently under Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
