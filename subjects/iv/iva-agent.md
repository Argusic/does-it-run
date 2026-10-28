# iva-agent

**Verdict: runs.** Argusic Score 94 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/smixs/iva-agent, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/iva-agent

## Pinned environment

- Project commit: `b2cabffbb147a75358d6f4ca4d8d22efdc06d2a3`
- Test commit: `b2cabffbb147a75358d6f4ca4d8d22efdc06d2a3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 63.8 to 63.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 94 | 35 | 63.8 | 10 | 7 | [run](https://argusic.com/run/f03efc80-09ce-4a7e-a655-c80e60860584) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18.x installed, project requires 24.x`
- 1 min: `uv not available for Python/graph tests`
- 3 min: `repair-shell: same-mtime files confuse bash -nt (versions 0.4.1 and 0.4.2)`
- 2 min: `memory-lock test: dash echo eats -n flag from fake flock script`
- 2 min: `brain-alerts test: hardcoded /opt/homebrew/bin/uv path`
- 1 min: `rollup-client test: dash echo eats -n flag from fake flock script`
- `same-inode ABA test fails on overlayfs (container metadata ctime)`
- `card-store-resolve test: module-level cache leaks between test files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
