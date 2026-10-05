# rom

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hanakai-rb/rom, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/run/74014d2b-b854-4b5f-92f5-d551f249936c

## Pinned environment

- Project commit: `7bee6fe337f689674fca1e260787176b17fc885d`
- Test commit: `7bee6fe337f689674fca1e260787176b17fc885d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 27.8 to 61.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 61.6 | 0 | 0 | [run](https://argusic.com/run/74014d2b-b854-4b5f-92f5-d551f249936c) |
| 2 | pass | 100 | 22 | 27.8 | 6 | 6 | [run](https://argusic.com/run/075872ad-fc57-403d-8a3a-481d9838efcf) |

## What was observed on a clean machine

Attempt 2:

- 12 min: `Ruby not installed in container (ruby: not found)`
- 5 min: `psych (YAML) extension failed to compile during initial Ruby build (missing libyaml headers)`
- 3 min: `zlib extension failed to compile during initial Ruby build (missing zlib headers)`
- 1 min: `gem command unusable because psych and zlib extensions were not loaded`
- 1 min: `Bundler failed on git source rom-sql (git source not checked out)`
- 3 min: `PostgreSQL not available for tests requiring DB connection (PG::ConnectionBad)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
