# spree

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spree/spree, licensed BSD-3-Clause, written in Ruby.

Evidence and recordings: https://argusic.com/subject/spree

## Pinned environment

- Project commit: `8bf7b07219854ab9643a97376091b53bc8a6831f`
- Test commit: `8bf7b07219854ab9643a97376091b53bc8a6831f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.9 to 6.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 6.9 | 1 | 1 | [run](https://argusic.com/run/f047d831-7933-4f62-8eb9-95b5aba4bed5) |

## What was observed on a clean machine

Attempt 1:

- `Ruby backend (spree/core, spree/api, etc.) requires Ruby >= 3.2, PostgreSQL, and bundler , none available in this container and cannot be installed without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
