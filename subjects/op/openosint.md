# OpenOSINT

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenOSINT/OpenOSINT, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/openosint

## Pinned environment

- Project commit: `a0a525376c38538b78e389e8a313b221400df3fb`
- Test commit: `a0a525376c38538b78e389e8a313b221400df3fb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.8 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 6.8 | 3 | 3 | [run](https://argusic.com/run/d22f0ef6-f214-47a9-8cdd-5baa20dc1dac) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `sublist3r binary not found (search_domain tool) causing one test assertion failure`
- 3 min: `Wrong sherlock package installed (distributed locking library sherlock != sherlock-project)`
- 2 min: `holehe and sherlock-project not installed causing 2 person-playbook test failures`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
