# cc-safety-net

**Verdict: runs.** Argusic Score 86.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kenryu42/cc-safety-net, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cc-safety-net

## Pinned environment

- Project commit: `af34a34ba0a04ea631d5910b2ddfc2cdc35bd8cd`
- Test commit: `af34a34ba0a04ea631d5910b2ddfc2cdc35bd8cd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.9 to 14.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 5 | 14.9 | 3 | 1 | [run](https://argusic.com/run/2495d2fd-d4f7-4984-91c5-579c733d2489) |

## What was observed on a clean machine

Attempt 1:

- `dist/ files used ES module import/export syntax but no dist/package.json with type=module , E2E tests failed`
- `Pre-existing: tests/cli/doctor/text.test.ts - 'text doctor shows active custom rules' returns exit 1`
- `Pre-existing: tests/core/io/safe-read.test.ts - 'replaces an existing file, gives it the write mode' expects mode 420 but gets 436`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
