# Vibe-Workflow

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SamurAIGPT/Vibe-Workflow, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/vibe-workflow

## Pinned environment

- Project commit: `121bde4ef0499ea000be98bdeaf1b244b928a8f3`
- Test commit: `121bde4ef0499ea000be98bdeaf1b244b928a8f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.2 to 16.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 16.2 | 3 | 3 | [run](https://argusic.com/run/f01d5f9d-c338-4d73-9c6b-f4ebcaff1783) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 too old for Next.js 16 (requires >=20.9.0)`
- 5 min: `MuAPI external API key required`
- 1 min: `Mock API returned wrapped object but frontend expected bare array for get-workflow-defs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
