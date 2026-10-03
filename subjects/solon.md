# solon

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/opensolon/solon, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/solon

## Pinned environment

- Project commit: `f465f0bda9b0fe801fcd490b7eb05ca993815507`
- Test commit: `f465f0bda9b0fe801fcd490b7eb05ca993815507`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.7 to 26.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26 | 26.7 | 3 | 3 | [run](https://argusic.com/run/a2361a76-befe-49d0-9e4b-8deeecdb5650) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Java or Maven pre-installed`
- 2 min: `solon-config-yaml tests fail: PropAddLoadTest and PropUtilTest use assertions on Properties.toString() order which differs between JDK 8 and JDK 17`
- `Full __test suite: 51/98 test classes fail (211/441 tests) due to test isolation issues: shared @SolonTest(App.class) state, HTTP server port conflicts, and JDK 17 incompatibilities`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
