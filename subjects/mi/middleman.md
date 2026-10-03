# middleman

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/middleman/middleman, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/middleman

## Pinned environment

- Project commit: `ec3eab8d7540ec474a8ae187bd466fafe8e147ad`
- Test commit: `ec3eab8d7540ec474a8ae187bd466fafe8e147ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 37.6 to 37.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 34 | 37.6 | 5 | 5 | [run](https://argusic.com/run/3dc7a4e4-498f-4ab6-93cc-edffd8777343) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Ruby not found in container`
- 3 min: `libyaml-0.so.2 missing - native extensions failed to build for psych gem`
- 2 min: `ruby header files not found , mkmf couldn't build native extensions for bigdecimal, racc, etc.`
- 2 min: `rsync not found - fixture setup in RSpec and cucumber tests failed`
- 1 min: `bundler version mismatch , lockfile requires 2.6.2, container had 2.4.19`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
