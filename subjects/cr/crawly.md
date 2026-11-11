# crawly

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elixir-crawly/crawly, licensed Apache-2.0, written in Elixir.

Evidence and recordings: https://argusic.com/subject/crawly

## Pinned environment

- Project commit: `e27f032285bdd9aaae27f27cccbe25fcc556dfd8`
- Test commit: `e27f032285bdd9aaae27f27cccbe25fcc556dfd8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 0.2 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 0.2 | 0 | 0 | [run](https://argusic.com/run/22ad8a8a-0fae-4285-ba9e-9308004a08df) |
| 2 | pass | 100 | 11 | 11.3 | 4 | 4 | [run](https://argusic.com/run/bc0598aa-847d-4157-a560-6872d4d3d0e1) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `Erlang/OTP runtime not installed in container (no erl, erlc, escript binaries)`
- 1 min: `Erlang erl scripts hardcode ROOTDIR=/usr/lib/erlang which doesn't exist in container`
- 1 min: `Missing erlang-public-key OTP app (public_key.app, BEAM files)`
- 1 min: `Leftover dets_simple_storage file from mix run pollutes test state causing failures on re-runs`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
