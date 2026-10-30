# adritian-free-hugo-theme

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zetxek/adritian-free-hugo-theme, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/adritian-free-hugo-theme

## Pinned environment

- Project commit: `924e081ed87cea0c81002897ed22fe77074319ea`
- Test commit: `924e081ed87cea0c81002897ed22fe77074319ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.1 to 20.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 52 | 20.1 | 5 | 5 | [run](https://argusic.com/run/59dc36a3-002f-443c-8396-740a477dc415) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Hugo binary not found in container`
- 2 min: `Go binary not found (required by Hugo modules)`
- 3 min: `Node.js v18 too old for png-to-ico ESM module (requires >=20)`
- 1 min: `RTL visual snapshot blog-post-ltr.png had 2px height difference from font metrics`
- `npm test OOM when running build+scripts+e2e main+e2e no-menus concurrently`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
