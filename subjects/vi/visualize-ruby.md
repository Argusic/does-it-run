# visualize_ruby

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zeisler/visualize_ruby, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/visualize-ruby

## Pinned environment

- Project commit: `5ecdd2b33afb1abb8784772f3d66d07c085020f5`
- Test commit: `5ecdd2b33afb1abb8784772f3d66d07c085020f5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.6 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4.6 | 3 | 3 | [run](https://argusic.com/run/09bb03d4-4051-4d56-93c5-325cb0109030) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Ruby interpreter or gem in container; ruby/gem not found`
- 2 min: `bundle install failed building native gem bigdecimal 4.1.3: conda Ruby required x86_64-conda-linux-gnu-cc compiler which was missing`
- 1 min: `require "visualize_ruby" from a standalone script raised LoadError since the gem was not installed system-wide`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
