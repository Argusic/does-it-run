# deconz-rest-plugin

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dresden-elektronik/deconz-rest-plugin, licensed BSD-3-Clause, written in C++.

Evidence and recordings: https://argusic.com/subject/deconz-rest-plugin

## Pinned environment

- Project commit: `a4c17adfa04abc63637ad17de7f85256a825a2cb`
- Test commit: `a4c17adfa04abc63637ad17de7f85256a825a2cb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.4 to 25.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 25.4 | 9 | 9 | [run](https://argusic.com/run/0646c0b8-2e60-4f3b-a665-66db4e96cd80) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Qt6 development packages not installed`
- 1 min: `ninja not available`
- 3 min: `FindOpenGL could not find GL libraries`
- 1 min: `Qt6DBus lib not in prefix`
- 2 min: `Catch2 v2.13.1 fails on GCC 13`
- 1 min: `deconz headers not in include path`
- 1 min: `SKIP_EMPTY_PARTS undefined for test libs`
- 1 min: `resource lib missing deCONZLib link`
- 1 min: `device_js CMakeLists had nonexistent files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
