# spreadsheet_architect

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/westonganger/spreadsheet_architect, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/spreadsheet-architect

## Pinned environment

- Project commit: `658702d4db294a174d04f6472f7795fad6dc7efb`
- Test commit: `658702d4db294a174d04f6472f7795fad6dc7efb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 13 | 3 | 3 | [run](https://argusic.com/run/70d6f499-dd98-479d-ae7b-8b295f6fd8ba) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Ruby not installed in container`
- 2 min: `zlib extension not compiled with Ruby (missing dev headers)`
- 2 min: `psych/yaml extension not compiled (missing libyaml)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
