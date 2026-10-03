# chat-on-steroids

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/totec448-spec/chat-on-steroids, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/chat-on-steroids

## Pinned environment

- Project commit: `3c0578fb02c0f41d22a1fe492988fda9dde20b41`
- Test commit: `3c0578fb02c0f41d22a1fe492988fda9dde20b41`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23 to 23 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.3 | 23 | 1 | 1 | [run](https://argusic.com/run/e6c43d23-491f-4be7-8389-a02971f37a3e) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `Node.js v18.19.1 too old , the project requires ^22.12.0 || ^24.0.0 || >=26.0.0 (vitest, vite, jsdom, undici and others all reject v18)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
