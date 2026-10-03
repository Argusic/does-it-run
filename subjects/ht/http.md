# http

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/httprb/http, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/http

## Pinned environment

- Project commit: `a210c0adb724b340121cafcbceccd7424e7e25e4`
- Test commit: `a210c0adb724b340121cafcbceccd7424e7e25e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.3 to 21.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 21.3 | 4 | 4 | [run](https://argusic.com/run/2de1db2b-aff7-4cae-8095-fe12593b1b41) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Ruby not found`
- 1 min: `zlib.h not found (bundler requires zlib)`
- 2 min: `psych native extension not built (RubyGems YAML parser)`
- `Gemfile 'ruby RUBY_VERSION' resolved to 3.4.0.dev, mismatch with runtime 3.4.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
