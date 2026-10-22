# pasteguard

**Verdict: runs with mocks.** Argusic Score 85.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sgasser/pasteguard, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pasteguard

## Pinned environment

- Project commit: `114c11b7f695f7711a477cedf5c3c8a8b89c647f`
- Test commit: `114c11b7f695f7711a477cedf5c3c8a8b89c647f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 38.2 to 38.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 85.33 | 37 | 38.2 | 3 | 2 | [run](https://argusic.com/run/668741dd-fca5-4f8b-9536-8a279cd478b5) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Bun installer failed: unzip not installed`
- 12 min: `uring-charge model urchade/gliner_multi_pii-v1 fails to load under pinned transformers/tiktoken: 'Error parsing line b\'\x0e\' in .../spm.model' (tiktoken cannot convert mdeberta spm slow-model tokenizer to fast; model repo has no tokenizer`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
