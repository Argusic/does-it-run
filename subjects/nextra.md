# nextra

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shuding/nextra, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nextra

## Pinned environment

- Project commit: `d6e80e1dd627b781429a6ee989b15ebba688c8ea`
- Test commit: `d6e80e1dd627b781429a6ee989b15ebba688c8ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.3 to 16.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 16.3 | 4 | 4 | [run](https://argusic.com/run/4686814f-f9ad-4015-8335-af141bdb84c8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `corepack was not available on Node v18.19.1, cannot enable via corepack enable`
- 1 min: `nextra DTS build failed with JS heap out of memory (Worker OOM)`
- 1 min: `3 vitest tests timed out at default 17000ms timeout`
- `snapshot mismatch in to-page-map test: new typesense/page.mdx file in docs/ example`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
