# hermes-desktop

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fathah/hermes-desktop, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hermes-desktop

## Pinned environment

- Project commit: `2ed89070bc6c9e8231a37bb55df8a7722a3776b8`
- Test commit: `2ed89070bc6c9e8231a37bb55df8a7722a3776b8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19.6 to 19.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 19.6 | 3 | 3 | [run](https://argusic.com/run/07489770-ffb5-43a7-8d7f-9ed3e15aac85) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node 18.19.1 is too old: @electron/get is ESM-only and fails with ERR_REQUIRE_ESM on postinstall`
- 5 min: `OPENROUTER_API_KEY in global process.env contaminates resolvedSecretMap() causing config-health test to falsely pass`
- 1 min: `Lint prettier warnings from edited test file`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
