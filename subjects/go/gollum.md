# gollum

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gollum/gollum, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/gollum

## Pinned environment

- Project commit: `d00fefc89be0ab22ab862a51299120a55ccd9280`
- Test commit: `d00fefc89be0ab22ab862a51299120a55ccd9280`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.2 to 16.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17 | 16.2 | 3 | 3 | [run](https://argusic.com/run/20cc72b0-0290-4fad-8666-30a4d7d8ab72) |

## What was observed on a clean machine

Attempt 1:

- 13 min: `Ruby not available in container (no ruby binary found)`
- 2 min: `Ruby zlib standard extension failed to build during compile (missing zlib.h / no -fPIC .a)`
- 2 min: `Ruby psych (YAML) extension failed to build (missing libyaml headers and lib)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
