# deja-vu

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vshulcz/deja-vu, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/deja-vu

## Pinned environment

- Project commit: `17f3878e54281727856cf87cf4ac645006c4366f`
- Test commit: `17f3878e54281727856cf87cf4ac645006c4366f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 59.2 to 59.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 59.2 | 4 | 4 | [run](https://argusic.com/run/e8bd4d36-38c7-4ec6-93f1-d2b05c6109ad) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No Go toolchain in container; CI pins Go 1.25.x, so the repo could not build or test out of the box`
- 12 min: `TestFilesCommandHonoursTrustPolicy failed: 'deja files' scoped to the cwd project never surfaced a synced peer session (project 'imported:svc') whose file was in the same repo, even under an allow-imported policy, because the widening branc`
- 6 min: `TestDeepSeekAutoDigestContract failed: generated dsh plugin files were ESM (import/export) written as .js; Node 18 loaded them as CommonJS and threw 'Cannot use import statement outside a module'`
- 2 min: `TestInstallingTheMissingToolMakesTheIndexStale failed because the container had neither sqlite3 nor zstd CLIs, so a store built 'without tools' was indistinguishable from today, and the environment-gated sqlite3 index/incremental tests were`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
