# qm-music

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chenqimiao/qm-music, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/qm-music

## Pinned environment

- Project commit: `e14547e15540a3038b5d915aadb9fcd6b566a4bc`
- Test commit: `e14547e15540a3038b5d915aadb9fcd6b566a4bc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.5 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 12.9 | 3 | 3 | [run](https://argusic.com/run/b413f841-517f-4f8c-8fcd-de111300b115) |
| 2 | pass | 100 | 8 | 9.5 | 0 | 0 | [run](https://argusic.com/run/615e1d19-46f8-4b75-968c-904ca1215eb9) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Java and Maven not installed in container`
- 1 min: `Maven download from dlcdn.apache.org returned 404 HTML page`
- 0.5 min: `Runtime directories dev-db/, music_dir/, cache/ missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
