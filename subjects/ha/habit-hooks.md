# habit-hooks

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/habit-hooks/habit-hooks, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/habit-hooks

## Pinned environment

- Project commit: `5603331f8c31b1537761e6639f49b876acf0a4e4`
- Test commit: `5603331f8c31b1537761e6639f49b876acf0a4e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.7 to 17.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18.3 | 17.7 | 3 | 3 | [run](https://argusic.com/run/3b405dbc-ffdc-41e4-9bc2-cb9b804cb0eb) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `jscpd ERR_REQUIRE_ESM on Node v18`
- 5 min: `pmd not on PATH (no JRE/PMD installed)`
- 3 min: `Java test test_a_ruleset_named_in_args_is_still_honoured failed - PMD 7.12 ExcessiveParameterList uses > not >= for minimum`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
