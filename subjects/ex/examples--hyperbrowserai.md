# examples

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hyperbrowserai/examples, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/7bcf4ae3-8a1e-46ef-beb9-55ad512df39e

## Pinned environment

- Project commit: `742df66242aad1ad5474b817909d1e85f953168f`
- Test commit: `742df66242aad1ad5474b817909d1e85f953168f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12 to 12 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.2 | 12 | 2 | 2 | [run](https://argusic.com/run/7bcf4ae3-8a1e-46ef-beb9-55ad512df39e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `The quick-start CLI (company-researcher.ts) is readline/TTY-only; piping stdin made it print the two prompts then exit code 0 before ever calling Hyperbrowser, so it could not be exercised non-interactively.`
- 1 min: `The app had no way to target a non-default API endpoint, so it could not be pointed at a local mock to verify end-to-end without real credentials.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
