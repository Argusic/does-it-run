# claudexor

**Verdict: runs.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/razzant/claudexor, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/claudexor

## Pinned environment

- Project commit: `529e512f5f112af9009dea55d0b2c2d08b57b6a5`
- Test commit: `529e512f5f112af9009dea55d0b2c2d08b57b6a5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 19.8 to 85.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 84 | 85.3 | 3 | 0 | [run](https://argusic.com/run/79d89f9b-2b33-42b3-8f8b-f4a8c7d1cd6e) |
| 2 | pass | 100 | 5 | 19.8 | 3 | 3 | [run](https://argusic.com/run/eb2c476e-ccad-4615-91f1-0d78fcd8be7b) |

## What was observed on a clean machine

Attempt 1:

- `legacy-writer-claimant.test.ts fails: requires git tag v3.3.7 not present in shallow checkout`
- `orchestrator.test.ts hangs due to interactive subprocess spawning`
- `cli-run-contract.test.ts hangs in batch due to interactive subprocess`

Attempt 2:

- 1 min: `Node.js v18.19.1 installed but project requires >=20.19.0`
- 1 min: `pnpm not found (corepack unavailable on Node 18)`
- 1 min: `git tag v3.3.7 missing from shallow clone, causing 1 test failure in legacy-writer-claimant.test.ts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
