# zero2Agent

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ranxi2001/zero2Agent, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/zero2agent

## Pinned environment

- Project commit: `39094a8db5e71bc0ef1d1f7f26240536484834d6`
- Test commit: `39094a8db5e71bc0ef1d1f7f26240536484834d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 6 | 6.5 | 5 | 0 | [run](https://argusic.com/run/1e9ba9ab-2f98-4844-bbab-1820f5bf2ee7) |

## What was observed on a clean machine

Attempt 1:

- `Python PEP 668 prevents pip install of PyYAML and other packages`
- `Ruby/Jekyll not installed; bundle exec jekyll build unavailable`
- `pandoc and xelatex not installed; PDF rebuild not possible`
- `mmdc (mermaid CLI) not installed; mermaid syntax validation skipped`
- `5 pre-existing test failures in classify-interview-questions/ (semantic recall mappings out of sync with question-index data)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
