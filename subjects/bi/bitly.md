# bitly

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/philnash/bitly, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/bitly

## Pinned environment

- Project commit: `3fb9585c255819028b670ec2a6353e3bf91c4ad1`
- Test commit: `3fb9585c255819028b670ec2a6353e3bf91c4ad1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.5 to 10.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 10.5 | 4 | 4 | [run](https://argusic.com/run/c87909e9-0f84-4a83-9649-e14212743a51) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `No Ruby interpreter in container`
- 3 min: `Native extensions failed: mkmf can't find ruby.h (no ruby-dev headers)`
- 3 min: `psych.so missing libyaml-0.so.2 / readline.so missing libncurses.so.6`
- 4 min: `OAuth access_token under WebMock: faraday-net_http 3.5.0 incompatible with webmock 3.7.6 (wrong number of arguments (given 2, expected 1))`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
