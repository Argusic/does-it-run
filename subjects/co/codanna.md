# codanna

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bartolli/codanna, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/codanna

## Pinned environment

- Project commit: `58295d290f70c2ca46a5ace48fe2aab8687d7d6e`
- Test commit: `58295d290f70c2ca46a5ace48fe2aab8687d7d6e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.1 to 27.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.2 | 27.1 | 1 | 1 | [run](https://argusic.com/run/82c9e24c-12e4-4db8-a739-f0105f7dcd49) |

## What was observed on a clean machine

Attempt 1:

- `19 watcher/unified tests and 5 CLI tests fail: 'Failed to initialize watcher: Too many open files (os error 24)'. Inotify instances limited to 128.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
