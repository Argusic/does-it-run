# agy-fast

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/INK-Q/agy-fast, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agy-fast

## Pinned environment

- Project commit: `fe635e1e06c856fff2e85e3f4fc4b3828da2ef3e`
- Test commit: `fe635e1e06c856fff2e85e3f4fc4b3828da2ef3e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8.2 to 27 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.7 | 27 | 5 | 5 | [run](https://argusic.com/run/53b3de25-32c1-4ecf-818a-4c898a9ffa14) |
| 2 | pass | 100 | 11 | 8.2 | 2 | 2 | [run](https://argusic.com/run/be589244-6360-4dda-ae19-1979493b7a1a) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `System Node.js is v18.19.1 but project requires >=20`
- 0.1 min: `esbuild native binary compiled for older glibc not compatible with Node.js 20`
- 5 min: `test/session-start.test.ts tests 9-10 cancelledByParent - fs.readdir module mock broken after esbuild bundling`
- 0.3 min: `test/mcp-protocol.test.ts test 1 timed out after 10s when running full suite`
- 0.3 min: `test/updater.test.ts test 5 assertion failure when run with other suites - expected 'updated' got 'error' due to resource contention`

Attempt 2:

- 2 min: `Node.js v18.19.1 installed, project requires >=20`
- 5 min: `Two session-start tests cancelled: monkey-patched fs.readdir used t.unref() on 300ms setTimeout, unsettled Promise tripped Node test runner`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
