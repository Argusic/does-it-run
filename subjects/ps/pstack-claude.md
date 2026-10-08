# pstack-claude

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/michael-denyer/pstack-claude, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/pstack-claude

## Pinned environment

- Project commit: `c02fd4922b25ee005f42042463d741d236c2c35e`
- Test commit: `c02fd4922b25ee005f42042463d741d236c2c35e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 3.4 | 2 | 2 | [run](https://argusic.com/run/8853165c-8926-4e36-b386-ede8ae5f6e23) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `bun not available on system (requires unzip for shell installer)`
- 1 min: `skills@1.5.23 CLI requires Node >= 22.20.0 but system has Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
