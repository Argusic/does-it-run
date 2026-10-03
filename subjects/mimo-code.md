# MiMo-Code

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/XiaomiMiMo/MiMo-Code, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mimo-code

## Pinned environment

- Project commit: `849ca66cc8debbbcc08904039e05bd2e79be348d`
- Test commit: `849ca66cc8debbbcc08904039e05bd2e79be348d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 18.3 to 37.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 18.3 | 0 | 0 | [run](https://argusic.com/run/f7d8d5f2-3ba2-4332-b4ce-56b878d757e1) |
| 2 | pass | 100 | 5.3 | 37.4 | 6 | 6 | [run](https://argusic.com/run/76a951d1-41dd-4c6f-898d-dca7a5b35eea) |

## What was observed on a clean machine

Attempt 2:

- 1.5 min: `Bun not available in container`
- 0.5 min: `'write.test.ts' expects 0o644 file mode, got 0o664`
- `'collapse.test.ts' Hangul jamo width: Bun.stringWidth returns 2, test expects 4`
- `'checkpoint-writer-wait-timeout.test.ts': 10 tests fail when grouped, 0 fail individually`
- `'node-migration.test.ts' 2 failures: Node build pipeline not set up`
- `'session-list-visibility.test.ts': 1 fail grouped, passes individually`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
