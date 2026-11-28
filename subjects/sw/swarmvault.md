# swarmvault

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/swarmclawai/swarmvault, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/swarmvault

## Pinned environment

- Project commit: `815412d24298e59e5073ded1ddd6c0e6aee9b91b`
- Test commit: `815412d24298e59e5073ded1ddd6c0e6aee9b91b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.9 to 6.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 6.9 | 2 | 2 | [run](https://argusic.com/run/337c38b8-f6b7-454b-a741-95e3efe92850) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node v18.19.1 too old (requires >=24) , pnpm install warned unsupported engine`
- 0.5 min: `npm install -g pnpm failed with EACCES on /usr/local/lib/node_modules`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
