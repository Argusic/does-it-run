# trustgraph

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/trustgraph-ai/trustgraph, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/trustgraph

## Pinned environment

- Project commit: `61524b78b29726ede12d27f41cb41a763a227ed8`
- Test commit: `61524b78b29726ede12d27f41cb41a763a227ed8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 11.4 to 18.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 18.5 | 3 | 3 | [run](https://argusic.com/run/f1a99526-65f8-4f19-bed0-c90b0cb4bf6d) |
| 2 | pass with mocks | 92 | 15 | 11.4 | 3 | 3 | [run](https://argusic.com/run/406419fe-3b8e-4f5c-8a10-6c5f10be75f0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Python is externally managed (PEP 668)`
- 3 min: `Editable install finders fragment trustgraph namespace between packages`
- 1 min: `8 tests failed due to missing sentence-transformers`

Attempt 2:

- 3 min: `Missing *__version__*_version.py files in all trustgraph packages (gitignored, not in repo)`
- 2 min: `Debian externally-managed Python environment blocked system-wide pip install`
- 5 min: `Editable pip install of namespace packages caused trustgraph-flow to shadow other packages' sub-modules`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
