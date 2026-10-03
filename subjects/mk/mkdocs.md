# mkdocs

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mkdocs/mkdocs, licensed BSD-2-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/mkdocs

## Pinned environment

- Project commit: `2862536793b3c67d9d83c33e0dd6d50a791928f8`
- Test commit: `2862536793b3c67d9d83c33e0dd6d50a791928f8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.4 to 4.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 4.4 | 1 | 1 | [run](https://argusic.com/run/4032bd93-c255-4f50-a6f9-88c26f7d801c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `2 test failures in test_draft_docs_with_comments_from_user_guide: PathSpec lines with leading whitespace caused pathspec to produce a no-op pattern set`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
