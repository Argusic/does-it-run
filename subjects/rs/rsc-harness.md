# rsc-harness

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ericrisco/rsc-harness, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/rsc-harness

## Pinned environment

- Project commit: `726aaf3ba87c584329fc821f243a7ce5e62450fd`
- Test commit: `726aaf3ba87c584329fc821f243a7ce5e62450fd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 29.7 to 29.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 29.7 | 3 | 3 | [run](https://argusic.com/run/8946c16c-fd62-4bc7-be47-035edcdad626) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `import.meta.dirname not available in Node.js v18 (used in 4 test files)`
- 1 min: `awk {2,3} quantifier not supported in mawk (used in skills/implement/scripts/task-brief)`
- 1 min: `Cannot use import statement outside a module: OpenCode plugin .js files loaded from temp dirs without package.json type:module`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
