# thulite

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/thuliteio/thulite, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/thulite

## Pinned environment

- Project commit: `1a445c196ad39430fd57a2bc56dd483d096081ae`
- Test commit: `1a445c196ad39430fd57a2bc56dd483d096081ae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4 | 3 | 3 | [run](https://argusic.com/run/8564d9bf-175a-4844-95f7-266d6564c64a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Hugo extended binary not found on system`
- 1 min: `Dart Sass not found on system`
- 1 min: `Node.js v18 on PATH is too old; Hugo 0.166.0's PostCSS pipeline passes --permission and --allow-fs-read flags to node, which only exist in Node 23+`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
