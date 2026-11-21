# git-fame-rb

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/oleander/git-fame-rb, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/git-fame-rb

## Pinned environment

- Project commit: `f94948c5867384c2aa48d299bff987fd233a0e27`
- Test commit: `f94948c5867384c2aa48d299bff987fd233a0e27`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.4 to 30.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.4 | 5 | 5 | [run](https://argusic.com/run/dc3df67b-abb3-428a-ad17-d17371af48f3) |
| 2 | pass | 100 | 30 | 30.3 | 4 | 4 | [run](https://argusic.com/run/cef84df6-0eac-45ba-9116-28fc5b21ac56) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Ruby not installed in container`
- 4 min: `Ruby build failed on missing dev headers (zlib1g-dev, libyaml-dev, libffi-dev)`
- 1 min: `Bundler failed with 'cannot load such file -- zlib'`
- 1 min: `psych extension failed to load (missing libyaml)`
- 1 min: `fiddle extension build failed (libffi.a not compiled with -fPIC)`

Attempt 2:

- 13 min: `Ruby 3.3 not installed in container`
- 3 min: `zlib C extension not compiled during Ruby build (missing -dev headers)`
- 5 min: `psych YAML C extension not compiled (missing libyaml dev headers)`
- 1 min: `psych.so could not find libyaml-0.so.2 at runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
