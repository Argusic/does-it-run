# ruby-openai

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alexrudall/ruby-openai, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/ruby-openai

## Pinned environment

- Project commit: `62938e02bb83e9f243ad2447805bc461d5d126fe`
- Test commit: `62938e02bb83e9f243ad2447805bc461d5d126fe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.6 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 16.6 | 5 | 5 | [run](https://argusic.com/run/e1c47451-3ac1-42ca-aac5-b24f665d6a8b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Ruby not installed in container`
- 1 min: `libruby-3.2.so.3.2 not found on library path`
- 1 min: `libyaml-0.so.2 not found (RubyGems requires it)`
- 2 min: `Ruby header files not found (native ext gems require ruby.h)`
- 1 min: `Bundler version mismatch (lockfile 2.4.5, installed 4.0.22)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
