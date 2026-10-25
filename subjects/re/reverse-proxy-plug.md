# reverse_proxy_plug

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tallarium/reverse_proxy_plug, licensed MIT, written in Elixir.

Evidence and recordings: https://argusic.com/subject/reverse-proxy-plug

## Pinned environment

- Project commit: `fbf373155bf9299676338a344e9369a3f35bc8f3`
- Test commit: `fbf373155bf9299676338a344e9369a3f35bc8f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.3 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 9.3 | 4 | 4 | [run](https://argusic.com/run/911560be-ed10-4315-bb49-83a5bc53f2b9) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Elixir and Erlang not found on system PATH`
- 3 min: `mix local.hex fails: ssl.app not found`
- 2 min: `earmark_parser xrl compilation fails: leexinc.hrl not found`
- 1 min: `Protocol consolidation fails: could not write to consolidated/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
