# brisa

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/brisa-build/brisa, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/brisa

## Pinned environment

- Project commit: `555b635d281cd13a2f62416191e4f14c00aab1d9`
- Test commit: `555b635d281cd13a2f62416191e4f14c00aab1d9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 73.6 to 73.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 74 | 73.6 | 4 | 4 | [run](https://argusic.com/run/95b07b0a-1ecf-4033-bb65-cb23ff4bd0f9) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `bun not installed in container (requires bun>=1.3.0; bun.lock present)`
- 38 min: `bun 1.4.3 build fails: 'Bun.build cannot be called from within a macro during bundling' (bundler deadlock restriction)`
- 20 min: `bun 1.3.0 build is flaky: recurring bun segfaults/SIGABRT ('panic: Segmentation fault', bun bug, random steps)`
- 12 min: `Full test suite hangs on pinned bun 1.3.0 (bun test-runner deadlock on certain files, e.g. cli/build.test.ts, compile-all) and ~10 pre-existing failures are identical on pristine code`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
