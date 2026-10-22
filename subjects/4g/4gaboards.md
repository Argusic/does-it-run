# 4gaBoards

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RARgames/4gaBoards, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/4gaboards

## Pinned environment

- Project commit: `82875e7687f65c8de22f9f34320ce7f934fa3291`
- Test commit: `82875e7687f65c8de22f9f34320ce7f934fa3291`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.3 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.3 | 5 | 5 | [run](https://argusic.com/run/0a378b5b-de92-4e0a-b039-d56d6bd9e645) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Node v18.19.1 installed but project requires ^24.11`
- 2 min: `sharp native module built for Node 18, fails on Node 24`
- 4 min: `PostgreSQL not available in container`
- 1 min: `.npmrc engine-strict=true blocked pnpm on Node 18`
- `camelcase ES module require() fails in jest fileTransform with Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
