# claude-chat-exporter

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agarwalvishal/claude-chat-exporter, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/claude-chat-exporter

## Pinned environment

- Project commit: `ab8de7d1ec67ae33f3570cbdc7658802f6e8d61c`
- Test commit: `ab8de7d1ec67ae33f3570cbdc7658802f6e8d61c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 24 to 24 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 24 | 3 | 3 | [run](https://argusic.com/run/2e099f50-41f0-4399-b8e9-a6d520596cb7) |

## What was observed on a clean machine

Attempt 1:

- 18 min: `jsdom runtime gap: no window.fetch and Node-18 fetch rejects relative URLs`
- 22 min: `jsdom leaves URL.createObjectURL unimplemented and Node's built-in URL.createObjectURL rejects jsdom Blobs (instanceof)`
- 2 min: `host sh lacks a login shell substitution pattern for backgrounded commands`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
