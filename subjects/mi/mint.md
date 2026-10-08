# mint

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elixir-mint/mint, licensed Apache-2.0, written in Elixir.

Evidence and recordings: https://argusic.com/subject/mint

## Pinned environment

- Project commit: `fb850d3714e4d79b9112d8056fe87cfd96b84f21`
- Test commit: `fb850d3714e4d79b9112d8056fe87cfd96b84f21`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.5 to 12.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 12.5 | 4 | 4 | [run](https://argusic.com/run/2ca0b1a6-b78d-4c57-a36b-cfbb1feec91e) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Erlang/OTP not installed (no erl, elixir, or mix in PATH)`
- 2 min: `Elixir not installed (Ubuntu version 1.14 but project requires ~> 1.15)`
- 1 min: `Test suite failed to start: could not find application file: tools.app`
- 1 min: `Test suite failed to start: could not find application file: xmerl.app`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
