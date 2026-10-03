# DEEIX-Chat

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DEEIX-AI/DEEIX-Chat, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/deeix-chat

## Pinned environment

- Project commit: `16450dbc41769a4930df475d2aec6c1b435c1cfe`
- Test commit: `16450dbc41769a4930df475d2aec6c1b435c1cfe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.1 to 23.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 11.1 | 4 | 4 | [run](https://argusic.com/run/f8ba6e81-aa54-4b10-8ec0-d9c62f36af02) |
| 2 | pass | 100 | 21 | 23.2 | 5 | 5 | [run](https://argusic.com/run/ca202e53-4e59-4f74-9207-cba2a09035ce) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26.8 not installed in container`
- 1 min: `sqlite3 development headers not installed (libsqlite3-dev missing)`
- 1 min: `pnpm not installed`
- 1 min: `pnpm install failed on mermaid ENOTEMPTY`

Attempt 2:

- 2 min: `Go 1.26 compiler not found in container`
- 1 min: `pnpm not available; npm install -g failed due to permissions`
- 2 min: `libsqlite3-dev headers/libs missing for CGO`
- 1 min: `Node.js 18 too old for Next.js 16 (needs >=20.9.0)`
- 2 min: `pnpm isolated linker hid tailwindcss-oxide native .node binary from turbopack bundler`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
