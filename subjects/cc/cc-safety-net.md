# cc-safety-net

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kenryu42/cc-safety-net, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cc-safety-net

## Pinned environment

- Project commit: `af34a34ba0a04ea631d5910b2ddfc2cdc35bd8cd`
- Test commit: `af34a34ba0a04ea631d5910b2ddfc2cdc35bd8cd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.9 to 33.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 5 | 14.9 | 3 | 1 | [run](https://argusic.com/run/2495d2fd-d4f7-4984-91c5-579c733d2489) |
| 2 | pass | 100 | 2 | 33.9 | 5 | 5 | [run](https://argusic.com/run/ca2c7a44-3f0d-42ad-bb99-a5deb87ab545) |

## What was observed on a clean machine

Attempt 1:

- `dist/ files used ES module import/export syntax but no dist/package.json with type=module , E2E tests failed`
- `Pre-existing: tests/cli/doctor/text.test.ts - 'text doctor shows active custom rules' returns exit 1`
- `Pre-existing: tests/core/io/safe-read.test.ts - 'replaces an existing file, gives it the write mode' expects mode 420 but gets 436`

Attempt 2:

- 2 min: `Bun was not pre-installed in the environment; needed unzip which wasn't available apt-get installable without root`
- 15 min: `10 test failures (6 packed-runtime, 2 Pi e2e, 2 OpenCode e2e, 2 Hermes e2e) caused by buildRuntimeBundles not writing a package.json with type:module at the output root , Node.js could not load ES module output files in temp directories`
- 5 min: `linked worktree facts test failure , git config parser didn't detect unterminated double-quoted strings (backslash-escaped final quote), returning a wrong path instead of null like real git`
- 3 min: `atomic policy writes test failure , writeFileSync respects umask (002), creating the test fixture at 0o664 instead of expected 0o644`
- 1 min: `text doctor shows active custom rules , pre-existing failure (exit code 1 instead of 0) not caused by my changes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
