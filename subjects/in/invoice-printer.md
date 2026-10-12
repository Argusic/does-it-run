# invoice_printer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/strzibny/invoice_printer, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/invoice-printer

## Pinned environment

- Project commit: `511e891d8a77d582ea2e5ec39e50f4aa32e76e8f`
- Test commit: `511e891d8a77d582ea2e5ec39e50f4aa32e76e8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.5 | 10 | 3 | 3 | [run](https://argusic.com/run/bd8c2db8-3998-48e5-ae04-d12c094ab71e) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `Ruby 3.3.12 build failed: missing libffi-dev, libyaml-dev, zlib1g-dev headers and shared libraries`
- 0.2 min: `bundle install failed: benchmark group gem rmagick requires ImageMagick development headers`
- 0.2 min: `Server returned 400 on render with example JSON due to non-Windows-1252 characters (ř, ž, etc.)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
