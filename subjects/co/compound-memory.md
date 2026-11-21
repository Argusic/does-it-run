# compound-memory

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Protocol-zero-0/compound-memory, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/compound-memory

## Pinned environment

- Project commit: `937080747f60e6eb44b83fdef1e0addcbee1a560`
- Test commit: `937080747f60e6eb44b83fdef1e0addcbee1a560`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.4 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 8.4 | 3 | 3 | [run](https://argusic.com/run/f2a5f523-e83f-404d-894f-37f988cd261d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `cm doctor crashed: crontab not installed, subprocess FileNotFoundError in _crontab_read/_crontab_write`
- 2 min: `mini_yaml parser returns string '{}' instead of empty dict for labels: {}`
- 1 min: `lexicon._overrides() crashes with AttributeError: 'str' object has no attribute 'items' on string '{}'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
