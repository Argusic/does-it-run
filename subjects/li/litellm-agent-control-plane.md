# litellm-agent-control-plane

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LiteLLM-Labs/litellm-agent-control-plane, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/litellm-agent-control-plane

## Pinned environment

- Project commit: `53bfd20e2fec51fc8f665fb614512c6b138367da`
- Test commit: `53bfd20e2fec51fc8f665fb614512c6b138367da`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 0.3 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 8.1 | 0 | 0 | [run](https://argusic.com/run/28479c84-63c6-488b-89fa-55336274556f) |
| 2 | fail | 20 | n/a | 0.3 | 0 | 0 | [run](https://argusic.com/run/92bc6a4f-2ac2-4ce3-a010-0160a9797ccd) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
