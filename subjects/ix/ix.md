# Ix

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ix-infrastructure/Ix, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ix

## Pinned environment

- Project commit: `f36c4e0fc96af715364db5c35ad2a723398433a6`
- Test commit: `f36c4e0fc96af715364db5c35ad2a723398433a6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.2 to 25.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 9.2 | 2 | 2 | [run](https://argusic.com/run/443adde6-088f-4b89-8e7c-cba929d2a6de) |
| 2 | pass | 95 | 20 | 25.5 | 4 | 3 | [run](https://argusic.com/run/34617dab-cdd0-4fc1-bbfc-04b82601bcc7) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 installed but project requires >=22.0.0`
- `Docker not installed in container (required for backend services)`

Attempt 2:

- 3 min: `Node.js 18 installed, project requires >=22.0.0`
- 2 min: `Tree-sitter native addons segfaulted (prebuilt for Node 18 ABI)`
- 2 min: `Core-ingestion vitest fails: missing @rolldown/binding-linux-x64-gnu`
- 1 min: `1 test times out: ingest-files.test.ts requires Docker backend`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
