# fess

**Verdict: could not verify.** Argusic Score 47.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/codelibs/fess, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/fess

## Pinned environment

- Project commit: `78abc12b37f764fcf14543b137f372440fdbd42b`
- Test commit: `78abc12b37f764fcf14543b137f372440fdbd42b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 35.9 to 79 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 4 | 79 | 3 | 3 | [run](https://argusic.com/run/c9fc419b-d18a-4479-8540-df58955830a4) |
| 2 | fail | 45 | 35 | 35.9 | 4 | 3 | [run](https://argusic.com/run/bfd05a9b-af65-479f-a3da-c5146dd314b1) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Java and Maven not pre-installed`
- 2 min: `Parent POM fess-parent:15.9.0-SNAPSHOT not resolvable offline`
- `Fess's SuggestHelper.init() fails with search_phase_execution_exception: No mapping found for [_shard_doc] in order to sort on`

Attempt 2:

- 3 min: `Java not installed`
- 1 min: `Maven not installed`
- 1 min: `unzip not installed`
- `OpenSearch 3.8.0 binary (1 GB) could not be downloaded over slow connection`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
