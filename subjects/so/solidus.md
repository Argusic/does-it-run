# solidus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/solidusio/solidus, licensed BSD-3-Clause, written in Ruby.

Evidence and recordings: https://argusic.com/subject/solidus

## Pinned environment

- Project commit: `851dd55293262db3236c3484289e15499507c1fb`
- Test commit: `851dd55293262db3236c3484289e15499507c1fb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 42.3 to 42.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 42.3 | 7 | 7 | [run](https://argusic.com/run/f99edfd9-8716-4ad6-9975-f91a1f661bd4) |

## What was observed on a clean machine

Attempt 1:

- 7 min: `Ruby 3.2 missing from container`
- 2 min: `libyaml-0.so.2 missing for psych.so`
- 1 min: `yaml.h missing for psych native extension build`
- 5 min: `Native extensions failed: bindir and header paths pointed to /usr`
- 3 min: `Linker couldn't find libruby-3.2.so during extension builds`
- 4 min: `URI::RFC2396_PARSER missing in Ruby 3.2 (needed by Rails 8.1)`
- 2 min: `bundle install re-failed due to cached failed builds`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
