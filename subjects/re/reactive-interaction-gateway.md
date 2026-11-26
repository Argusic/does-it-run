# reactive-interaction-gateway

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Accenture/reactive-interaction-gateway, licensed Apache-2.0, written in Elixir.

Evidence and recordings: https://argusic.com/subject/reactive-interaction-gateway

## Pinned environment

- Project commit: `b65435c63db0572e7a0ed5acba08198c0bed7439`
- Test commit: `b65435c63db0572e7a0ed5acba08198c0bed7439`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 24.3 to 39.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 65 | 24.3 | 7 | 7 | [run](https://argusic.com/run/cd117e8f-4a60-47be-8a77-be98f1487056) |
| 2 | pass with mocks | 92 | 42 | 39.9 | 7 | 7 | [run](https://argusic.com/run/b4110305-5ce2-4d0f-a959-1afddfc825f5) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `No Erlang/Elixir runtime in container`
- 3 min: `Elixir version constraint in mix.exs rejects >=1.12`
- 10 min: `ssl_verify_fun fails to compile via mix erlc due to -include_lib path resolution`
- 2 min: `ex2ms 1.6.0 removed ':vars' key in macro env for Elixir 1.18`
- 3 min: `prometheus_ex 3.0.5 uses removed 'Kernel.Utils.defdelegate'`
- 10 min: `pg2 module removed in OTP 25`
- `47 test failures (8 crypto deprecation, 37+ infra-dependent)`

Attempt 2:

- 42 min: `Required Erlang 23.2.2 and Elixir 1.11.3 not pre-installed; built Erlang 26.2.5 from source and installed Elixir 1.15.4 precompiled`
- 5 min: `Missing dev dependencies for building Erlang (libncurses-dev, libssl-dev, autoconf) - no root access; installed via extracted .deb packages`
- 1 min: `ssl_verify_fun 1.1.6 incompatible with OTP 26 (record types removed)`
- 1 min: `prometheus_ex incompatible with Elixir 1.15 (Kernel.Utils.defdelegate removed)`
- 1 min: `ex2ms 1.6.0 incompatible with Elixir 1.15 (compile error in ExRated dep)`
- 5 min: `Ancient Cowboy/Ranch incompatible with OTP 26 TLS 1.3 (next_protocols_advertised option)`
- `19 test failures remain in full suite (port conflicts with FakeServer, HTTPS disabled, test ordering)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
