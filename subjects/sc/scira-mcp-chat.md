# scira-mcp-chat

**Verdict: runs.** Argusic Score 97.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zaidmukaddam/scira-mcp-chat, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/scira-mcp-chat

## Pinned environment

- Project commit: `c9467dc212fc3574fd813fb18dcdb0a044d095c2`
- Test commit: `c9467dc212fc3574fd813fb18dcdb0a044d095c2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 37.5 to 37.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 97.14 | 30 | 37.5 | 7 | 6 | [run](https://argusic.com/run/5e1843b2-6b0c-4fed-80d7-06946c296b72) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Build failed: Can't resolve 'zod/v3' (package.json pinned zod 3.23.8, but AI SDK's zod-to-json-schema@3.24.6 imports zod/v3)`
- 8 min: `Build failed: @tailwindcss/oxide native binding missing after npm install (npm optional-deps bug + node 18 EBADENGINE)`
- 3 min: `Turbopack build worker died: JavaScript heap out of memory during type check`
- 2 min: `Type error from ./node_modules.bak/@eslint/config-helpers (leftover npm node_modules shadowed the build)`
- 6 min: `DB endpoints returned 500: @neondatabase/serverless driver is WebSocket-only and cannot reach a local Postgres`
- 6 min: `Build failed Can't resolve 'tls'/'net'/'fs': client component chat.tsx imported DB code via lib/chat-store`
- 1 min: `/api/chat chat-streaming returns 500: request is gated by Vercel BotId OIDC (x-vercel-oidc-token + external bot-protection API) before any AI provider key is used`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
