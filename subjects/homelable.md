# homelable

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Pouzor/homelable, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/homelable

## Pinned environment

- Project commit: `d656a6a07f4a89c637bbfe285ab7d5a8573823aa`
- Test commit: `d656a6a07f4a89c637bbfe285ab7d5a8573823aa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 49.8 to 57.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 49.8 | 0 | 0 | [run](https://argusic.com/run/8f0d5077-b225-4aa9-ab8d-c3082e952e17) |
| 2 | pass | 100 | 1 | 57.6 | 1 | 1 | [run](https://argusic.com/run/d51c6e9e-6c85-41fe-8cba-7657ccbb9cdc) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `MCP_API_KEY env var in .env.example is not declared in Settings model, causing pydantic ValidationError on startup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
