# zx

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/google/zx, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/zx

## Pinned environment

- Project commit: `65fc542d88baac578967e22bea28cb610976578c`
- Test commit: `65fc542d88baac578967e22bea28cb610976578c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.3 to 24.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 24.3 | 4 | 4 | [run](https://argusic.com/run/287a6111-a9ea-46c5-a7f4-77a0086f5800) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `CLI silently produced no output: isMain() always returned false on Node.js because import.meta.main is undefined (Deno-only)`
- 3 min: `core test failed: Promise.withResolvers is not a function (Node 22+ API, container runs Node 18)`
- `log.test.ts failures when NO_COLOR=1 env is set (chalk colors suppressed, tests expect ANSI)`
- `cli.test.js hangs after test 16 due to stale TCP connection in fakeServer (test 17 fake server's 500 response leaves dangling conn)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
