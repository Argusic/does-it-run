# parklife

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/benpickles/parklife, licensed MIT, written in Ruby.

Evidence and recordings: https://argusic.com/subject/parklife

## Pinned environment

- Project commit: `022b3ea7b91721489dbebafeef251162cc5162da`
- Test commit: `022b3ea7b91721489dbebafeef251162cc5162da`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 4.3 | 4 | 4 | [run](https://argusic.com/run/7a0a45a3-df3f-4720-b671-c9214c40b98b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Ruby not installed in container`
- 2 min: `Missing libyaml-0.so.2 for psych.so (gem command)`
- 2 min: `Missing ruby header files for native gem extensions`
- 3 min: `Test failure: Thor set_color returns plain text due to TERM=dumb and NO_COLOR=1 env`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
