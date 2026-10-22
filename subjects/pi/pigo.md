# pigo

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/smallnest/pigo, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/pigo

## Pinned environment

- Project commit: `891d1f372cefa92b5f5a104db20521238ba5a9fe`
- Test commit: `891d1f372cefa92b5f5a104db20521238ba5a9fe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 21 to 21 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 47 | 21 | 3 | 3 | [run](https://argusic.com/run/86133a65-6bb9-4f07-88ae-0fd9e8a1e96c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No Go toolchain in container (go.mod requires go 1.27rc1); no root to apt-install`
- 20 min: `Real LLM credentials absent; documented local-Ollama path requires a running daemon (connection refused on 11434)`
- 3 min: `pigo --provider ollama rejected (ollama is a model-id prefix, not a registry provider name)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
