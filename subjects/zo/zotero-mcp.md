# zotero-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/54yyyu/zotero-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/zotero-mcp

## Pinned environment

- Project commit: `075cf2c59842c0f195d25aeef87d3475254ef70b`
- Test commit: `075cf2c59842c0f195d25aeef87d3475254ef70b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 10.7 to 21.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 10.7 | 1 | 1 | [run](https://argusic.com/run/b12e7514-b031-456b-afe2-47f9c575753f) |
| 2 | pass with mocks | 92 | 3 | 21.7 | 1 | 1 | [run](https://argusic.com/run/82302d40-a389-4535-9d22-65a69997bdd3) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `test_stringified_params.py fixture leaks ZOTERO_LOCAL=true via os.environ.setdefault without cleanup, causing test_webdav::test_download_attachment_file_falls_back_to_webdav to fail`

Attempt 2:

- 5 min: `test_download_attachment_file_falls_back_to_webdav failed: test_stringified_params.py pollutes ZOTERO_LOCAL env var globally, causing is_local_mode() to return True and adding an extra 'Local storage: ...' error before the expected 'Local Z`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
