# slack-mcp-server

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/korotovsky/slack-mcp-server, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/slack-mcp-server

## Pinned environment

- Project commit: `b88c0de3f706f4f07337c9eda7133c736d1c9524`
- Test commit: `b88c0de3f706f4f07337c9eda7133c736d1c9524`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 9.9 to 15.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 15.2 | 0 | 0 | [run](https://argusic.com/run/bd8eff04-c5d1-4c57-8b66-d52ec0524f5e) |
| 2 | pass | 100 | 6 | 9.9 | 2 | 2 | [run](https://argusic.com/run/b8929a1f-fb43-430f-aee2-3e26b130748a) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
