# finch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sneako/finch, licensed MIT, written in Elixir.

Evidence and recordings: https://argusic.com/subject/finch

## Pinned environment

- Project commit: `3387d4be15d2d56ad18e878e62bea0e354385f15`
- Test commit: `3387d4be15d2d56ad18e878e62bea0e354385f15`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 11.7 | 4 | 4 | [run](https://argusic.com/run/6c3c10df-4b46-4f86-8c3a-03d412d1b46e) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `No Elixir/Erlang toolchain installed in container (elixir/erl not on PATH)`
- 1 min: `OTP tar had no bin/erl until install script run`
- 1 min: `Elixir bin scripts (mix, elixir, iex) lacked execute bit after unzip`
- 2 min: `mix test flaky failures (3 timing-sensitive tests) under parallel load: assert_receive ... 500ms races; run1 clean 234 passed, runs2-3 had 1-2 flaky failures each`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
