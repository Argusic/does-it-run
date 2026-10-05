# nanoc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nanoc/nanoc, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/nanoc

## Pinned environment

- Project commit: `10191952d0814f206a8d8b21cd5d0da3463e47ce`
- Test commit: `10191952d0814f206a8d8b21cd5d0da3463e47ce`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.2 to 44.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 41 | 44.2 | 9 | 9 | [run](https://argusic.com/run/35768f9a-8a9a-4483-bde5-c18b229da5a4) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No Ruby runtime in container`
- 3 min: `RubyGems not in LOAD_PATH by default`
- 2 min: `libyaml-0.so.2 missing (required by psych.so)`
- 4 min: `Ruby headers not found (mkmf.rb can't find ruby.h)`
- 1 min: `libruby-3.2.so linker symlink missing`
- 4 min: `rbtree native extension has undefined assert symbol`
- 1 min: `zeitwerk eager_load fails because Date/Time not yet loaded`
- 10 min: `Several plugin native extensions fail to compile (psych, eventmachine, mini_racer)`
- 3 min: `Bundle install with full Gemfile fails on native ext compilation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
