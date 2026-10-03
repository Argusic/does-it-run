# Graft

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/trailhq/Graft, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/graft

## Pinned environment

- Project commit: `05760b07abc0e427f5af8ad378889ee402c5afc6`
- Test commit: `05760b07abc0e427f5af8ad378889ee402c5afc6`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 9.6 to 18.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 18.3 | 2 | 2 | [run](https://argusic.com/run/7da78e14-f9c3-42a1-916c-90d7513f1896) |
| 2 | pass | 100 | 4.5 | 11.3 | 2 | 2 | [run](https://argusic.com/run/4cdba5a6-b51c-4b64-ad7a-ab6a21a34098) |
| 3 | pass | 100 | 2.5 | 9.6 | 1 | 1 | [run](https://argusic.com/run/4f741261-c432-48e5-8128-8574e59c4a21) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `tree-sitter-kotlin native addon cannot compile: missing make/gcc and no linux-x64 prebuilds in package`
- 2 min: `Node.js v18 installed but package requires >=20`

Attempt 2:

- 2 min: `Installed Node.js 18.19.1, but project requires >=20`
- 0.5 min: `Test 'a process killed while holding the lock releases it' failed on Node 20 because top-level await in -e eval is not supported`

Attempt 3:

- 4 min: `Test 'a process killed while holding the lock releases it' (graph-refresh.test.ts:434) failed: 'node -e' with top-level await throws SyntaxError because Node 20's -e runs as CommonScript by default`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
