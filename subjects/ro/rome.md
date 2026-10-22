# rome

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rome-os/rome, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/rome

## Pinned environment

- Project commit: `6ff9addd3658db184b259ad846586e68d1a3e8db`
- Test commit: `6ff9addd3658db184b259ad846586e68d1a3e8db`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 53.9 to 53.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 53.9 | 3 | 3 | [run](https://argusic.com/run/f9a5ebf1-062c-411f-a7cd-0685d9b7ab3f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node on PATH was v18 with no pnpm; repo requires Node>=24 + pnpm 11.6, so pnpm install could not start`
- 13 min: `pnpm test:unit failed once with a single order-dependent failure in packages/web channels-settings-page.test.tsx (debounced PATCH missing routing/session fields)`
- 5 min: `OTLP metrics exporter retries getaddrinfo EAI_AGAIN rome-obs; boot warns 'failed to schedule sentinel_review'; no Docker so dev stack (pnpm dev:all / dashboard on 3000) unavailable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
