# reactive-interaction-gateway

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Accenture/reactive-interaction-gateway, licensed Apache-2.0, written in Elixir.

Evidence and recordings: https://argusic.com/subject/reactive-interaction-gateway

## Pinned environment

- Project commit: `b65435c63db0572e7a0ed5acba08198c0bed7439`
- Test commit: `b65435c63db0572e7a0ed5acba08198c0bed7439`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24.3 to 24.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 65 | 24.3 | 7 | 7 | [run](https://argusic.com/run/cd117e8f-4a60-47be-8a77-be98f1487056) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `No Erlang/Elixir runtime in container`
- 3 min: `Elixir version constraint in mix.exs rejects >=1.12`
- 10 min: `ssl_verify_fun fails to compile via mix erlc due to -include_lib path resolution`
- 2 min: `ex2ms 1.6.0 removed ':vars' key in macro env for Elixir 1.18`
- 3 min: `prometheus_ex 3.0.5 uses removed 'Kernel.Utils.defdelegate'`
- 10 min: `pg2 module removed in OTP 25`
- `47 test failures (8 crypto deprecation, 37+ infra-dependent)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
