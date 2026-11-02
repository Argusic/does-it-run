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
- Valid runs: 2; wall time 24.3 to 67.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 24.3 | 4 | 4 | [run](https://argusic.com/run/287a6111-a9ea-46c5-a7f4-77a0086f5800) |
| 2 | pass | 100 | 66 | 67.1 | 7 | 7 | [run](https://argusic.com/run/a1915804-dd8a-473d-af3a-9eabd56283b4) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `CLI silently produced no output: isMain() always returned false on Node.js because import.meta.main is undefined (Deno-only)`
- 3 min: `core test failed: Promise.withResolvers is not a function (Node 22+ API, container runs Node 18)`
- `log.test.ts failures when NO_COLOR=1 env is set (chalk colors suppressed, tests expect ANSI)`
- `cli.test.js hangs after test 16 due to stale TCP connection in fakeServer (test 17 fake server's 500 response leaves dangling conn)`

Attempt 2:

- 12 min: `CLI silently no-op on Node 18/20: isMain relied on import.meta.main (Node 24+) so autorun() never ran`
- 8 min: `test/core.test.js used Node 22-only assert.unreachable() and Promise.withResolvers()`
- 6 min: `npm test unit step needs Node 24 flag --experimental-transform-types, absent on Node 18.19.1`
- 8 min: `chalk color mismatch: container NO_COLOR=1 disabled ANSI so log.test.ts failed; FORCE_COLOR changed chalk.level breaking generated export.test.js`
- 4 min: `test/cli.test.js non-std-ext assertion hard-coded checkout path basename 'zx'`
- 5 min: `test:size exceeded limits by ~130 B due to isMain fix`
- 4 min: `test:npm failed on Node 18: node -e 'import ...' requires --input-type=module`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
