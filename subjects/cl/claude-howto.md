# claude-howto

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/luongnv89/claude-howto, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-howto

## Pinned environment

- Project commit: `188f468893231cbe4525f45e657d554746232072`
- Test commit: `188f468893231cbe4525f45e657d554746232072`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.25 | 3 | 1 | 1 | [run](https://argusic.com/run/7e1691b9-ebb3-4588-aee1-6ae7ac92fc08) |
| 2 | pass | 100 | 3 | 6.7 | 1 | 1 | [run](https://argusic.com/run/5539d1bb-5d09-4c17-8a3b-20163115e60f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 too old for Pele 1.6.0 (requires >=20)`

Attempt 2:

- 3 min: `System Node.js v18.19.1 is too old for Pele 1.6.0 (requires >= 20); 2 test failures in test_pele_renderer.py`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
