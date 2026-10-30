# memoket-kite

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/memoket/memoket-kite, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/memoket-kite

## Pinned environment

- Project commit: `c007108f926d19a73fd9fe159b82e376804304f2`
- Test commit: `c007108f926d19a73fd9fe159b82e376804304f2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.7 to 16.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 16.7 | 3 | 3 | [run](https://argusic.com/run/98ee7f69-bad1-4c2f-a625-0dcdaf5d9c79) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System pip install blocked by externally-managed-environment`
- 2 min: `9 test failures: o200k_base tokenizer encoding unavailable (tiktoken not installed)`
- 2 min: `Mock LLM extract returned wrong src IDs (regex captured whole | delimited line)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
