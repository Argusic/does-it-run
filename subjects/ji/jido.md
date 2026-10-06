# jido

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agentjido/jido, licensed Apache-2.0, written in Elixir.

Evidence and recordings: https://argusic.com/subject/jido

## Pinned environment

- Project commit: `6244d7691cbe79585afb9e15ea0aecf19b0316d6`
- Test commit: `6244d7691cbe79585afb9e15ea0aecf19b0316d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.9 to 15.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 15.9 | 2 | 2 | [run](https://argusic.com/run/4831bb3a-b43a-4f21-b5b3-6029db00a6b9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Erlang/OTP or Elixir runtime installed in container; apt packages too old and no sudo`
- 1 min: `mix deps.compile poolboy failed because rebar3 calls erl with hardcoded /usr/lib/erlang path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
