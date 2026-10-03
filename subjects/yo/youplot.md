# YouPlot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/red-data-tools/YouPlot, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/youplot

## Pinned environment

- Project commit: `e67219ca88ccdc5da9f14c4a346c24b8da8ce25c`
- Test commit: `e67219ca88ccdc5da9f14c4a346c24b8da8ce25c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.2 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10.1 | 10.2 | 3 | 3 | [run](https://argusic.com/run/17ea2942-9cfa-44f7-8b80-661d9483eefe) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Ruby not available (no system install)`
- 1 min: `gem3.2 failed: missing libyaml shared library`
- 2 min: `gem install unicode_plot failed: no ruby.h (missing ruby-dev)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
