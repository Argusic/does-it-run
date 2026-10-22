# cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/modelstudioai/cli, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/run/a1ad94fc-b423-475b-8c5b-8a0c6a50ea4b

## Pinned environment

- Project commit: `8bbbbc722d70fb200641ef22b6f6d033aeae9f74`
- Test commit: `8bbbbc722d70fb200641ef22b6f6d033aeae9f74`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.6 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 16.6 | 7 | 7 | [run](https://argusic.com/run/a1ad94fc-b423-475b-8c5b-8a0c6a50ea4b) |

## What was observed on a clean machine

Attempt 1:

- 35 min: `Header PowerShell script not found in shell`
- `calls.echo missing`
- `the run command uses the mock API`
- `connect ECONNREFUSED 127.0.0.1:18080`
- `dist bundles import src TS (strip-only cannot parse parameter properties)`
- `index signature`
- `Installer errors encountered`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
