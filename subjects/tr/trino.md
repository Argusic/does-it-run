# trino

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/trinodb/trino, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/trino

## Pinned environment

- Project commit: `4ccfb5aa84338d3fb923cd37ad5eb52b33dd381d`
- Test commit: `4ccfb5aa84338d3fb923cd37ad5eb52b33dd381d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 17.9 to 45.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 17.9 | 4 | 4 | [run](https://argusic.com/run/2fddb054-6ad9-497a-b369-4675fe4f7bcc) |
| 2 | pass | 100 | 41 | 45.2 | 1 | 1 | [run](https://argusic.com/run/3de5db03-9b13-4549-a274-1550045759d3) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Java runtime installed in container`
- `Docs build failed: Sphinx not installed (exit 127)`
- `jdk.incubator.vector module not enabled`
- `Port 8080 in use from prior crashed process`

Attempt 2:

- `trino-docs module failed: requires sphinx-build (exit 127)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
