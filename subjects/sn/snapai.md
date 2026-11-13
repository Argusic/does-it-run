# snapai

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Code-with-Beto/snapai, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/snapai

## Pinned environment

- Project commit: `a60d5393287cbf46794507e6ee0ff54d689d5976`
- Test commit: `a60d5393287cbf46794507e6ee0ff54d689d5976`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 4.3 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 5.5 | 3 | 3 | [run](https://argusic.com/run/b5d9c020-b3bd-4f2f-98c4-bf72aebe67c3) |
| 2 | pass with mocks | 92 | 1.5 | 4.3 | 3 | 3 | [run](https://argusic.com/run/54d92656-4bf8-43f4-b7db-5ef8ba0f40d6) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm not found in PATH`
- 1 min: `Google GenAI SDK does not support custom base URLs`
- 1 min: `Initial mock PNG had corrupt header for sharp resize`

Attempt 2:

- 0.5 min: `pnpm not available; repo uses pnpm-lock.yaml`
- 0.3 min: `tsc command not found after initial pnpm install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
