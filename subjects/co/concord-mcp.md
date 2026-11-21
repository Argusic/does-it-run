# concord-mcp

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Get-Concord-AI/concord-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/concord-mcp

## Pinned environment

- Project commit: `8f7b735a833daa2e2d4156df33be539a1bb3f3ee`
- Test commit: `8f7b735a833daa2e2d4156df33be539a1bb3f3ee`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 1.6 to 3.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 3.5 | 2 | 2 | [run](https://argusic.com/run/67f3435f-067b-4082-b676-8070ac6c2a83) |
| 2 | pass | 100 | 2 | 1.6 | 0 | 0 | [run](https://argusic.com/run/b4a1fa6c-6c00-4e83-a502-872858400c02) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `scaffold Node is v18.19.1 but package.json engines requires Node >=22.12, and pnpm is not installed (node_modules and dist absent)`
- 1 min: `pnpm demo fails: 'Missing required command: tmux' (examples/whack-a-mole/run.sh)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
