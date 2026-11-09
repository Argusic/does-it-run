# dsh-context

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bowenliang123/dsh-context, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dsh-context

## Pinned environment

- Project commit: `da01f29ca6602b78cf88f4921f41a5b95685d4c9`
- Test commit: `da01f29ca6602b78cf88f4921f41a5b95685d4c9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 2.1 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.1 | 0 | 0 | [run](https://argusic.com/run/be309b4b-e276-433c-88e5-87d70ad5c933) |
| 2 | pass with mocks | 92 | 3 | 3.2 | 0 | 0 | [run](https://argusic.com/run/e841a25e-bc8f-4435-a894-824d35df01ee) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
