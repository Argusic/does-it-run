# Free-LLM

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nejib1/Free-LLM, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/free-llm

## Pinned environment

- Project commit: `194eaa6b1938d109c6cf77646a42123831704ac6`
- Test commit: `194eaa6b1938d109c6cf77646a42123831704ac6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 0.9 to 1.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0 | 0.9 | 0 | 0 | [run](https://argusic.com/run/fe2147c3-6b90-43aa-a700-0734f62fe12b) |
| 2 | pass with mocks | 92 | 0 | 1.3 | 0 | 0 | [run](https://argusic.com/run/f4323d10-01ee-46af-a2de-9ec4cf74fb04) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
