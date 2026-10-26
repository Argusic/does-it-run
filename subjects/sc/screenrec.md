# screenREC

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/heysagnik/screenREC, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/screenrec

## Pinned environment

- Project commit: `f811128318f76f790695444880d1420d3b0aba69`
- Test commit: `f811128318f76f790695444880d1420d3b0aba69`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 0.2 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 0.2 | 0 | 0 | [run](https://argusic.com/run/5981688d-7383-4b51-9173-aaed5de4dca7) |
| 2 | pass | 100 | 3 | 4.9 | 3 | 3 | [run](https://argusic.com/run/acda87e1-59c1-48ce-bf6c-e8b818098254) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `pnpm not found on PATH`
- 2 min: `Node.js 18.19.1 too old for Next.js 16 (needs >=20.9.0)`
- `next start failed to find .next build from wrong cwd`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
