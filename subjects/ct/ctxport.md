# ctxport

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nicepkg/ctxport, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ctxport

## Pinned environment

- Project commit: `c4e3db1be3191d4167d2218c90dd9cfbea0dc924`
- Test commit: `c4e3db1be3191d4167d2218c90dd9cfbea0dc924`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.5 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 21 | 8.5 | 2 | 2 | [run](https://argusic.com/run/518570f8-449a-4c7a-a1a4-7063c040ccc8) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `system Node was v18 and pnpm was absent, below both pnpm/npm engine requirements (node>=22, pnpm>=10)`
- 8 min: `core-markdown test failure: serializeConversation returned estimatedTokens=47 instead of 0 for an empty conversation (frontmatter was tokenized)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
