# kanba

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Kanba-co/kanba, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/kanba

## Pinned environment

- Project commit: `d5dfe822a503dcf87e14e687e4a13a0baffc9fe3`
- Test commit: `d5dfe822a503dcf87e14e687e4a13a0baffc9fe3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27.7 to 27.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 55 | 27.7 | 8 | 8 | [run](https://argusic.com/run/c183d2e0-93c0-4831-bc1a-73911b21d253) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Build failed: placeholder Supabase URL in .env.example is an invalid URL (ERR_INVALID_URL) during page-data collection for /api/stripe/webhook`
- 6 min: `Mock PostgREST filter parsing treated eq.X values as column names, so filters matched nothing`
- 6 min: `Mock returned empty arrays for embedded relations and dropped scalar columns on select=*,project_members!inner(role)`
- 10 min: `Mock .single() requests returned arrays, so project.id was undefined and the share page queried project_id=eq.undefined`
- 5 min: `Mock returned 405 for HEAD requests used by the slug-uniqueness check`
- 4 min: `Browser requests blocked by CORS because Accept-Profile header was not in mock's allowed list`
- 3 min: `Mock login failed because the Supabase JS client sends grant_type as a query parameter`
- 5 min: `Mock lacked notifications table, listener views, and realtime WebSocket handshake, causing console errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
