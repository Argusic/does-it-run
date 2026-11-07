# earshot

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Leonxlnx/earshot, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/earshot

## Pinned environment

- Project commit: `591fa3e028032e6dce56620a20e932e35667e8d8`
- Test commit: `591fa3e028032e6dce56620a20e932e35667e8d8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 32 to 32 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 32 | 1 | 1 | [run](https://argusic.com/run/9146a1e0-e3f0-495f-9ac2-99f6b9861d09) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `12 test_interfaces.py tests failed: FakeRequests SLEEP pollution from subprocess via global time.sleep monkeypatch (8 LLM tests) + missing 'mcp' module (4 MCP tests)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
