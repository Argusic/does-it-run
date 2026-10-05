# full-stack-ai-agent-template

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vstorm-co/full-stack-ai-agent-template, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/full-stack-ai-agent-template

## Pinned environment

- Project commit: `3428d9a6214619d3514312886d59a36400747b7d`
- Test commit: `3428d9a6214619d3514312886d59a36400747b7d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 37.2 to 37.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 37.2 | 3 | 3 | [run](https://argusic.com/run/0be22d35-d87b-4d62-a716-c773e29e5cc8) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `ResourceLimits key rename in pydantic-ai: max_duration_secs -> max_feed_duration_secs`
- 3 min: `get_agent() call used unsupported context= parameter`
- 4 min: `StreamedRunResult lacks stream_events() method and stream.result() is property not callable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
