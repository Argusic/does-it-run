# credit_card_validations

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/didww/credit_card_validations, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/credit-card-validations

## Pinned environment

- Project commit: `3857a44465f7bfda1670a50aeec917ae6da1c43c`
- Test commit: `3857a44465f7bfda1670a50aeec917ae6da1c43c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.3 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.3 | 3 | 3 | [run](https://argusic.com/run/c7bfd96f-1266-42aa-bafa-d990e60c3e98) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Ruby not installed in container`
- 3 min: `Ruby zlib extension not compiled (missing zlib1g-dev headers)`
- 3 min: `Ruby psych (YAML) extension not compiled (missing libyaml headers)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
