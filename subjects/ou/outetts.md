# OuteTTS

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/edwko/OuteTTS, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/outetts

## Pinned environment

- Project commit: `f5eac6e70d792844c6a6959d900a47af2c061a5b`
- Test commit: `f5eac6e70d792844c6a6959d900a47af2c061a5b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 14.6 to 14.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 14.6 | 3 | 3 | [run](https://argusic.com/run/c307b157-15b9-4f35-8891-184c94a4dcb3) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `version/interface.py eagerly imported all 6 backend model classes at module level, causing ImportError when any backend dependency was missing`
- `sounddevice fails at import: PortAudio library not found (system package libportaudio)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
