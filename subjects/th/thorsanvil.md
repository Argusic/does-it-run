# ThorsAnvil

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Loki-Astari/ThorsAnvil, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/thorsanvil

## Pinned environment

- Project commit: `679f2c1136293f0275a87f7a718c161aa085ee20`
- Test commit: `679f2c1136293f0275a87f7a718c161aa085ee20`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.9 to 44.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 44.9 | 8 | 8 | [run](https://argusic.com/run/d6fd180d-f55b-4586-8e4b-b95971722793) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing magic_enum.hpp header - project dependency not installed`
- 3 min: `Missing libyaml - required for YAML serialization`
- 2 min: `Missing libsnappy - required for compression support`
- 2 min: `Missing libz (zlib.h) - required for compression`
- 3 min: `Missing libevent - required for async IO event loop`
- 5 min: `Missing Boost >= 1.70 with coroutine2 support - required by Nisse`
- 2 min: `libyaml and libsnappy built without -fPIC causing shared library link failures`
- 5 min: `NisseBolt Slack test binary missing boost_context at link time due to -L path not including boost`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
