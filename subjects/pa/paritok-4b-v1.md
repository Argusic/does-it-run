# paritok-4b-v1

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Paritok-official/paritok-4b-v1, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/paritok-4b-v1

## Pinned environment

- Project commit: `c2ab50fc92fa5aa2fae3db1ce916d6d1a8e2980c`
- Test commit: `c2ab50fc92fa5aa2fae3db1ce916d6d1a8e2980c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 7.9 to 20.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 20.4 | 0 | 0 | [run](https://argusic.com/run/92673dcb-f4ca-4d74-9dee-c38b9b5fb4d9) |
| 2 | pass | 100 | 2 | 7.9 | 1 | 1 | [run](https://argusic.com/run/c065d72c-b51a-4bb8-998f-5f800afd0637) |

## What was observed on a clean machine

Attempt 2:

- `Ollama not available (no root). Compression model cannot be pulled.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
