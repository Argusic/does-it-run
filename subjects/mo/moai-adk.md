# moai-adk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/modu-ai/moai-adk, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/moai-adk

## Pinned environment

- Project commit: `7ad9f8534dc48719854c67e2b9a06db97b594eaf`
- Test commit: `7ad9f8534dc48719854c67e2b9a06db97b594eaf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 56.5 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/d633b3f1-ff3d-4704-906b-e4d5317cf20c) |
| 2 | pass | 100 | 40 | 56.5 | 3 | 3 | [run](https://argusic.com/run/00618d6b-fadf-418e-8d68-f0e9a480ae39) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `sg binary not in PATH (ast-grep sg CLI) , tests that exercise the real ast-grep scanner skipped`
- `TestCC_FactoryEntryThroughRunCC and TestGLM_FactoryWorkerEntry: test isolation bug , launchProjectRoot() uses resolveProjectDir() which ignores findProjectRootFn override, causing workers.json state pollution between subtests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
