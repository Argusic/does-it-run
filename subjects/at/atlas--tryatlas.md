# atlas

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tryatlas/atlas, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/run/0fb8100d-2783-45ef-bc30-c2da47e2ff1c

## Pinned environment

- Project commit: `ccac90f499f92b25bb0132305195ee3eeef9f6cf`
- Test commit: `ccac90f499f92b25bb0132305195ee3eeef9f6cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.1 to 18.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 18.1 | 4 | 4 | [run](https://argusic.com/run/0fb8100d-2783-45ef-bc30-c2da47e2ff1c) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `System Node.js v18.19.1 is too old , bun 1.4.4 reports Node 18 compat, and vitest 5 / rolldown need 'styleText()' from node:util (Node 21+)`
- 1 min: `Shallow git clone (no 'fetch-depth: 0') caused vendor-licensing.test.ts to fail`
- `dist/ directory had improper 0644 permissions (no execute bit), blocking rolldown output`
- 5 min: `The Tauri app (src-tauri) and its dependent crates cannot build on this Linux system , libwebkit2gtk-4.1-dev, libgtk-3-dev and friends are missing and cannot be installed (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
