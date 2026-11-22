# mcp-client-for-ollama

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jonigl/mcp-client-for-ollama, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mcp-client-for-ollama

## Pinned environment

- Project commit: `7322a9e425cb45cc6563ea108d07b345cac2b69e`
- Test commit: `7322a9e425cb45cc6563ea108d07b345cac2b69e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 4.4 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 5.8 | 1 | 1 | [run](https://argusic.com/run/a5080054-826a-4aab-b8e7-002e3c3c9302) |
| 2 | pass | 100 | 10 | 4.4 | 1 | 1 | [run](https://argusic.com/run/5fcb4b52-092a-4286-855f-ea5ee301718b) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Long unbroken JSON values were cropped with '...' by Rich Syntax word_wrap, hiding the _END tail of tool arguments/responses (2 failing tests)`

Attempt 2:

- 8 min: `Two tests failing in test_sanitize.py: TestNoWidthTruncation.test_long_argument_value_not_cropped and test_long_json_response_value_not_cropped , Rich Syntax word_wrap cannot break strings at whitespace mid-token, causing long values to be`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
