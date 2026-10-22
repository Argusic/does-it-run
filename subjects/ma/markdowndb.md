# markdowndb

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/flowershow/markdowndb, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/markdowndb

## Pinned environment

- Project commit: `f53cfef49ffcd267fc200d2dc451ed6f37b4523a`
- Test commit: `f53cfef49ffcd267fc200d2dc451ed6f37b4523a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 74.7 to 74.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 74.7 | 4 | 4 | [run](https://argusic.com/run/547b359f-a131-4d99-a22f-10e779971a9c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node 18.19.1 is below engines >=20; npm install printed EBADENGINE warning`
- 5 min: `MySQL backend needs optional peer mysql2, not auto-installed`
- 20 min: `Published registry tarball mddb@0.9.5 contains a stale 35-line CLI: npx mddb ./one ./two fails with 'Error loading configuration file' and no --exec/--help support`
- 5 min: `Config include/exclude globs are matched against absolute walk paths, so relative patterns like c1/** matched nothing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
