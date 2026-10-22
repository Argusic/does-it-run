# serviette

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pathwaycom/serviette, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/serviette

## Pinned environment

- Project commit: `fc9fa33a54f036a1d3529fa75315c1bcf57d23cb`
- Test commit: `fc9fa33a54f036a1d3529fa75315c1bcf57d23cb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 86 to 86 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.2 | 86 | 2 | 2 | [run](https://argusic.com/run/13ecb31e-bc7a-4de0-a080-6169b0fd5d78) |

## What was observed on a clean machine

Attempt 1:

- 55 min: `Pathway native Rust engine cryptographically validates license key (no demo key available without sign-in at pathway.com)`
- 5 min: `DuckDB subscribe-based mock initially stored all values as strings, causing ConversionException for numpy array embedding columns`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
