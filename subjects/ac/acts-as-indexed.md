# acts_as_indexed

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dougal/acts_as_indexed, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/acts-as-indexed

## Pinned environment

- Project commit: `2047215baa91d6f03e8cbf1396d69c7b2f500aa2`
- Test commit: `2047215baa91d6f03e8cbf1396d69c7b2f500aa2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.9 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 4.9 | 3 | 3 | [run](https://argusic.com/run/36daae6d-2ae3-42d9-b136-bf1252f43773) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Ruby 3.2.3 not installed in container`
- 1 min: `Shebangs in gem/bundle scripts hardcoded /usr/bin/ruby3.2`
- 1 min: `libyaml-0.so.2 missing for psych.so native extension`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
