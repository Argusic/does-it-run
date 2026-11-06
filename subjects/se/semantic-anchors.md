# Semantic-Anchors

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LLM-Coding/Semantic-Anchors, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/semantic-anchors

## Pinned environment

- Project commit: `1fd328552aae6d70141cfbbf156c903e29987b3d`
- Test commit: `1fd328552aae6d70141cfbbf156c903e29987b3d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.7 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 9.7 | 5 | 5 | [run](https://argusic.com/run/26c2b958-00c2-4d78-9f25-872c7e6ef653) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node system version 18.19.1 too old; all deps require Node 20+`
- 2 min: `@tailwindcss/oxide v4.2.1 missing linux-x64-gnu native binding on Node 18`
- 5 min: `html-encoding-sniffer uses CJS require() on ESM-only @exodus/bytes package causing ERR_REQUIRE_ESM in vitest fork workers`
- 1 min: `whatwg-url also uses CJS require() on @exodus/bytes ESM modules causing fork worker failures`
- 1 min: `scripts/ tests fail: rolldown native binding for linux-x64-gnu not installed as optional dependency`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
