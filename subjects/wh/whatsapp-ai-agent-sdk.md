# whatsapp-ai-agent-sdk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/csr1010/whatsapp-ai-agent-sdk, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/whatsapp-ai-agent-sdk

## Pinned environment

- Project commit: `9b1b02eb4ae47a8ad7850c3545bdaaa39b747a37`
- Test commit: `9b1b02eb4ae47a8ad7850c3545bdaaa39b747a37`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.2 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 2.2 | 3 | 3 | [run](https://argusic.com/run/9fb15e7c-b999-405f-a7a9-b3b251634df7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Container had Node.js 18 but project requires Node 22+`
- 2 min: `rolldown linux-x64 native binding missing after initial pnpm install under Node 18`
- 1 min: `pnpm not available in container, and npm global installs blocked by permissions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
