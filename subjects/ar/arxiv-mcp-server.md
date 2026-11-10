# arxiv-mcp-server

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/blazickjp/arxiv-mcp-server, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/arxiv-mcp-server

## Pinned environment

- Project commit: `42419c18376ef5559a38fa7f1895938ad2b84e38`
- Test commit: `42419c18376ef5559a38fa7f1895938ad2b84e38`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.9 to 2.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 1.9 | 0 | 0 | [run](https://argusic.com/run/6c024d79-7d03-44fd-b921-c48dcfff878f) |
| 2 | pass | 100 | 12 | 2.3 | 1 | 1 | [run](https://argusic.com/run/f99bcf87-991e-4be1-a403-4a5c0491a995) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `uv not preinstalled in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
