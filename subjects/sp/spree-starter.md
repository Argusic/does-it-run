# spree-starter

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spree/spree-starter, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/spree-starter

## Pinned environment

- Project commit: `584d0ec28161edf5ef9fe9eaad94a208e33fd55e`
- Test commit: `584d0ec28161edf5ef9fe9eaad94a208e33fd55e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.2 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 14.2 | 3 | 3 | [run](https://argusic.com/run/9931f83c-c498-473b-a92a-9752fcc75dab) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Ruby 4.0.1 not available in mise registry`
- 1 min: `mise gem plugin could not find 'mise' binary during bundle install`
- 3 min: `PostgreSQL 16 and client tools not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
