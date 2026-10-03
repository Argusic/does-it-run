# debezium

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/debezium/debezium, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/debezium

## Pinned environment

- Project commit: `841f3a72747e892c7ad8a1bf9f80206bbb8b1e15`
- Test commit: `841f3a72747e892c7ad8a1bf9f80206bbb8b1e15`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 64.5 to 64.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 31 | 64.5 | 3 | 3 | [run](https://argusic.com/run/e37b893d-f30d-4557-a07a-983ed397fcea) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Java runtime installed in container`
- 1 min: `debezium-storage-file jar error: NoSuchFileException for class file`
- 1 min: `debezium-sink maven-clean-plugin could not delete target`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
