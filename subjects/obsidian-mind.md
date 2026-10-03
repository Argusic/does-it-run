# obsidian-mind

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/breferrari/obsidian-mind, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/obsidian-mind

## Pinned environment

- Project commit: `af615d100a1d04561409ab9a1e71e615efa1d87b`
- Test commit: `af615d100a1d04561409ab9a1e71e615efa1d87b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 3.4 | 1 | 1 | [run](https://argusic.com/run/f0749bb9-7368-4b0d-8ad4-e44acdff44f2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node v18.19.1 lacks --experimental-strip-types required by TypeScript hook scripts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
