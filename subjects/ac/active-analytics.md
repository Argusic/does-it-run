# active_analytics

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BaseSecrete/active_analytics, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/active-analytics

## Pinned environment

- Project commit: `c63036148abf9b4c491ccc0d6940cdac1f2d3061`
- Test commit: `c63036148abf9b4c491ccc0d6940cdac1f2d3061`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 18.9 to 18.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 19 | 18.9 | 5 | 5 | [run](https://argusic.com/run/80cc7df1-7756-4cde-ae0f-83e27880ec0c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Ruby installed in container`
- 5 min: `Bundler version conflicts between site_ruby and default lib/ruby in Traveling Ruby`
- 3 min: `Gemfile.lock versions unavailable in pre-installed Traveling Ruby gems`
- 3 min: `No Redis server available for async queue tests`
- 1 min: `redis gem not pre-installed (only redis-client)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
