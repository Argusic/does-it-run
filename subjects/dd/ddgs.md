# ddgs

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deedy5/ddgs, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ddgs

## Pinned environment

- Project commit: `70a5635510fb8d5b15d5ba6ceced6a67e212149b`
- Test commit: `70a5635510fb8d5b15d5ba6ceced6a67e212149b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.2 to 12.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 1 | 12.2 | 1 | 0 | [run](https://argusic.com/run/a029bc02-8162-4ad8-832e-0b39e9e6d191) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `test_videos_search, test_videos_command, test_books_search, test_books_command fail , DuckDuckGo videos API and Anna's Archive return HTTP 403 from this container's IP`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
