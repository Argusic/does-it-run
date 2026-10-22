# probe

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/probelabs/probe, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/probe

## Pinned environment

- Project commit: `1ee1ecb7f459a8f83c63aa41d65d4bc1a7b6f5cf`
- Test commit: `1ee1ecb7f459a8f83c63aa41d65d4bc1a7b6f5cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.1 to 35.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 35.1 | 1 | 1 | [run](https://argusic.com/run/d04cecb2-feee-4acf-913e-ff5da6905b5d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing tests/schemas/json_output_schema.json , 4 schema validation tests failed to load the file`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
