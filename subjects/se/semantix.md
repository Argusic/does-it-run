# semantix

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Gnosil/semantix, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/semantix

## Pinned environment

- Project commit: `aad62b0b3f3ebdd8c0ed9454e7d5e11e6e603a67`
- Test commit: `aad62b0b3f3ebdd8c0ed9454e7d5e11e6e603a67`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 17.2 to 25.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 17.2 | 1 | 1 | [run](https://argusic.com/run/1e23a2b3-a739-4529-969b-130e26cdb503) |
| 2 | pass | 100 | 15 | 25.6 | 2 | 2 | [run](https://argusic.com/run/7282163a-cf4c-4875-9aac-82e1f83e2e1d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26+ not installed in container`

Attempt 2:

- 4 min: `Go runtime not installed in container - had to download Go 1.22.10 (which self-managed 1.26.5 toolchain)`
- `TestDurabilityFuzzCrashConsistency in harness/agent is flaky - fails under full parallel test suite but passes when run in isolation. Pre-existing timing-sensitive fuzz test.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
