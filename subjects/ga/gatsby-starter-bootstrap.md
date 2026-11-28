# gatsby-starter-bootstrap

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jaxx2104/gatsby-starter-bootstrap, licensed 0BSD, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/gatsby-starter-bootstrap

## Pinned environment

- Project commit: `beaa9231eb2005390d980b53280eb46013f38067`
- Test commit: `beaa9231eb2005390d980b53280eb46013f38067`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.3 to 21.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 21.3 | 4 | 4 | [run](https://argusic.com/run/7dae2de5-6dba-44e8-81d5-8937ba7254e1) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18 is installed but the project requires Node 22`
- 0.5 min: `pnpm is not installed`
- `Gatsby build was killed by OOM (exit 137) on first 3 attempts with 1GB RAM and no swap , at schema building phase with parallel workers`
- `textlint has no rules configured (no .textlintrc)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
