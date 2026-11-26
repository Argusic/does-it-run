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
- Valid runs: 2; wall time 29.7 to 66 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 29.7 | 3 | 3 | [run](https://argusic.com/run/8946c16c-fd62-4bc7-be47-035edcdad626) |
| 2 | pass | 100 | 0.1 | 66 | 6 | 6 | [run](https://argusic.com/run/893bcd3f-392c-457b-9baf-0026557f04d6) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `import.meta.dirname not available in Node.js v18 (used in 4 test files)`
- 1 min: `awk {2,3} quantifier not supported in mawk (used in skills/implement/scripts/task-brief)`
- 1 min: `Cannot use import statement outside a module: OpenCode plugin .js files loaded from temp dirs without package.json type:module`

Attempt 2:

- 5 min: `import.meta.dirname used in 4 test files is Node 21+ only, not available in Node 18.19.1`
- 8 min: `mawk v1.3.4 does not support {2,3} interval regex in skills/implement/scripts/task-brief (dead code path: heading matching never fired)`
- 4 min: `task-brief awk regex ([[:space:](]|-|$) didn't match em dash , after T002`
- 4 min: `ESM import from .js OpenCode plugin files failed with 'Cannot use import outside module' in 4 test files`
- 1 min: `Missing dirname import in 2 test files after import.meta.dirname fix`
- 1 min: `Missing fileURLToPath import in knowledge-sync and team-safe-default tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
