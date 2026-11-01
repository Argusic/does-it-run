# serviette

**Verdict: runs with mocks.** Argusic Score 61 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pathwaycom/serviette, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/serviette

## Pinned environment

- Project commit: `fc9fa33a54f036a1d3529fa75315c1bcf57d23cb`
- Test commit: `fc9fa33a54f036a1d3529fa75315c1bcf57d23cb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 41.3 to 86 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.2 | 86 | 2 | 2 | [run](https://argusic.com/run/13ecb31e-bc7a-4de0-a080-6169b0fd5d78) |
| 2 | fail | 30 | 2.5 | 41.3 | 1 | 0 | [run](https://argusic.com/run/e54b6368-2306-4a48-bfa9-9e9b14e9314b) |

## What was observed on a clean machine

Attempt 1:

- 55 min: `Pathway native Rust engine cryptographically validates license key (no demo key available without sign-in at pathway.com)`
- 5 min: `DuckDB subscribe-based mock initially stored all values as strings, causing ConversionException for numpy array embedding columns`

Attempt 2:

- 20 min: `Pathway requires a free license key from https://pathway.com/framework/get-license but the sign-up requires interactive GitHub/LinkedIn OAuth that cannot be automated in a headless container. The Pathway Rust engine binary (engine.abi3.so)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
