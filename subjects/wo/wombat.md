# wombat

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/felipecsl/wombat, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/wombat

## Pinned environment

- Project commit: `bd021b25c58735ffb94c1ce15623202215ed45a8`
- Test commit: `bd021b25c58735ffb94c1ce15623202215ed45a8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.2 to 12.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 12.2 | 3 | 3 | [run](https://argusic.com/run/978f1f6c-4491-48a0-bf8f-2821208d6ffd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Ruby runtime in container (ruby/gem/bundle not found)`
- 1 min: `libyaml-0.so.2 missing -> psych native extension and RubyGems failed to load`
- 2 min: `psych 5.3.1 native build failed: yaml.h header and libyaml.so symlink not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
