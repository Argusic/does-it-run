# scrapple

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AlexMathew/scrapple, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/scrapple

## Pinned environment

- Project commit: `0c19c7a2606f6ef5a1225a337c6ab08cb8431906`
- Test commit: `0c19c7a2606f6ef5a1225a337c6ab08cb8431906`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9.7 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 9.7 | 4 | 4 | [run](https://argusic.com/run/7becc32e-9a4e-41c0-9264-d33f60d78f20) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `nose 1.3.0 is Python 2-only and crashes on import under Python 3.12`
- 2 min: `selector.py uses Python 2 constructs: unicode type, itertools.izip, itertools.izip_longest`
- 1 min: `validate_config has operator precedence bug: %d % len(fields) - len(set(fields))`
- `4 run tests fail because external websites changed since 2018 (trakt.tv, basketball-reference.com, pyvideo.org)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
