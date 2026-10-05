# rom

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rom-rb/rom, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/run/12f257b5-2a5d-4e2f-b845-791e4728fd5e

## Pinned environment

- Project commit: `7bee6fe337f689674fca1e260787176b17fc885d`
- Test commit: `7bee6fe337f689674fca1e260787176b17fc885d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.6 to 26.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 26.6 | 7 | 7 | [run](https://argusic.com/run/12f257b5-2a5d-4e2f-b845-791e4728fd5e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Ruby not installed in container - no ruby binary, gem, or bundler`
- 6 min: `rubygems library files not in Ruby LOAD_PATH because rbconfig.rb had hardcoded /usr/ paths`
- 3 min: `Native extension builder subprocess could not find ruby3.2 (Gem.ruby returned /usr/bin/ruby3.2)`
- 3 min: `Native extension subprocesses lacked RUBYLIB, CPATH, C_INCLUDE_PATH environment`
- 2 min: `ext_conf_builder.rb cleared DESTDIR during make, breaking Makefile library search paths`
- 3 min: `gcc linker could not find -lruby-3.2 because CONFIG[archlibdir] resolved to /usr/lib/x86_64-linux-gnu`
- 5 min: `PostgreSQL server not available - all repository and changeset integration tests fail with connection refused`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
