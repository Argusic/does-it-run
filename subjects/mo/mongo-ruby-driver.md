# mongo-ruby-driver

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mongodb/mongo-ruby-driver, licensed Apache-2.0, written in Ruby.

Evidence and recordings: https://argusic.com/subject/mongo-ruby-driver

## Pinned environment

- Project commit: `6375dc607da5b3cbdf85d2c07aa1d2d9b0c6c29c`
- Test commit: `6375dc607da5b3cbdf85d2c07aa1d2d9b0c6c29c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.6 to 28.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 15.6 | 4 | 4 | [run](https://argusic.com/run/79c01482-915e-494e-bfbf-f3da62f94e53) |
| 2 | pass | 100 | 18 | 28.1 | 7 | 7 | [run](https://argusic.com/run/ae2df6a0-af35-4282-b92e-13d89a189d74) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Ruby not installed in the container`
- 2 min: `psych native extension failed to build (missing libyaml headers)`
- 5 min: `No MongoDB server available`
- 2 min: `Test suite authentication failures (root-user not found)`

Attempt 2:

- 8 min: `Ruby 3.2.6 not installed in container`
- 3 min: `libyaml missing - psych gem (required by RubyGems) couldn't load`
- 2 min: `zlib missing - bundler install failed without zlib`
- 3 min: `Ruby compiled with --with-static-linked-ext caused segfault in bigdecimal`
- 1 min: `git submodules not initialized (spec/shared)`
- 1 min: `MongoDB not running - test suite requires a running deployment`
- 1 min: `Default test users not created in MongoDB`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
