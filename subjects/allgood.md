# allgood

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rameerez/allgood, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/allgood

## Pinned environment

- Project commit: `b71d1cb5d29991a6197e9a20043532ce48b26bf4`
- Test commit: `b71d1cb5d29991a6197e9a20043532ce48b26bf4`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 23.7 to 23.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 23.7 | 5 | 5 | [run](https://argusic.com/run/fd4fad73-65a7-45d8-8c19-a62adf5c8545) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Ruby not installed in container`
- 5 min: `RubyGems not loaded - RUBYLIB path issue`
- 6 min: `C compilation fails - missing stdio.h (no glibc headers)`
- 3 min: `Prism superclass mismatch (bundled 0.19.0 vs gem 1.9.0)`
- 1 min: `Rate limit test failure due to CacheStore singleton leaking across test files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
