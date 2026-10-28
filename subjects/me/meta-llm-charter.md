# meta-llm-charter

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/entropyvortex/meta-llm-charter, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/meta-llm-charter

## Pinned environment

- Project commit: `7a814b1152ae1ae49202d172da477af5b345e2b9`
- Test commit: `7a814b1152ae1ae49202d172da477af5b345e2b9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 4.3 | 3 | 3 | [run](https://argusic.com/run/d81532c6-8ffc-4355-9e82-de7f61c1cbdd) |

## What was observed on a clean machine

Attempt 1:

- `npm audit reported 1 high severity advisory after install (no install failure)`
- 2 min: `fixture-local 'npm test' (node --import tsx) fails on container's Node 18.19.1: ERR_MODULE_NOT_FOUND for tsx; README/CI require Node 20+, canonical harness command is npx --yes tsx --test`
- `Full eval path 'npm start' cannot run: ANTHROPIC_API_KEY missing (harness abort by design), no docker binary/daemon available to build the sandbox image`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
