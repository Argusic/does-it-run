# invisible_dots

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/feder-cr/invisible_dots, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/invisible-dots

## Pinned environment

- Project commit: `5afd5f066ee708b2438652d706028b2716d993c8`
- Test commit: `5afd5f066ee708b2438652d706028b2716d993c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 48.6 to 48.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 48.6 | 1 | 1 | [run](https://argusic.com/run/219d5513-db53-4f1c-8d92-5a3bdbdc7d38) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Node.js v18.19.1 too old (project requires Node 24+); readline in Node 24.21 treats \u007f (DEL) literally on in-memory streams instead of as backspace`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
