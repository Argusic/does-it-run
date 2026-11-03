# haystack

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deepset-ai/haystack, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/haystack

## Pinned environment

- Project commit: `124b668001cdbe4258fbb7ce9e1da375bc430f39`
- Test commit: `124b668001cdbe4258fbb7ce9e1da375bc430f39`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.7 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 8.8 | 0 | 0 | [run](https://argusic.com/run/fd8114a8-3b44-4773-910d-06a89f91d3e8) |
| 2 | pass | 100 | 12 | 3.7 | 2 | 2 | [run](https://argusic.com/run/01145969-7a76-4720-a373-79a94bd90231) |

## What was observed on a clean machine

Attempt 2:

- 7 min: `Hatch not installed; system pip externally managed`
- 5 min: `test_pypdf_to_document::test_run_detect_paragraphs_to_be_used_in_split_passage failed , 'inter nal' vs 'internal' difference with pypdf 6.21.4`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
