# Wiki_MkDocs

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/linyuxuanlin/Wiki_MkDocs, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/wiki-mkdocs

## Pinned environment

- Project commit: `6a41dd3cf1eff364854064fcbaf6dce2ecb73565`
- Test commit: `6a41dd3cf1eff364854064fcbaf6dce2ecb73565`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.8 to 3.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 3.8 | 1 | 1 | [run](https://argusic.com/run/0898f37e-e3a0-4ed5-9fd9-913f4b2a063c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `mkdocs build crashed in mkdocs-rss-plugin git_manager/ci.py commit_count() with IndexError: list index out of range because the provisioned repo had zero git refs (detached FETCH_HEAD, no branches/tags), so for_each_ref() returned an empty`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
