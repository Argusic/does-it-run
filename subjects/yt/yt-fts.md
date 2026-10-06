# yt-fts

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NotJoeMartinez/yt-fts, licensed Unlicense, written in Python.

Evidence and recordings: https://argusic.com/subject/yt-fts

## Pinned environment

- Project commit: `7fbc0088f30672b6fbfe2ea7351fa42bafe1f886`
- Test commit: `7fbc0088f30672b6fbfe2ea7351fa42bafe1f886`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 18.7 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 18.7 | 7 | 7 | [run](https://argusic.com/run/f450bb5f-de1d-4188-b83d-ceee233e3aff) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `test_search.py did not load test database before tests; tests failed with no such table: Channels`
- 1 min: `test_search.py::test_global_search asserted YC Root Access which does not exist in test DB`
- 1 min: `test_export.py used subprocess.run("rm *.csv") without -f, crashing when no csvs existed`
- 8 min: `test_download.py used real yt-dlp calls which fail because YouTube changed channel layout; downloads yield 0 videos`
- 1 min: `test_download.py populate_jcs_channel referenced undefined loop variable i`
- 1 min: `test_download.py::test_channel_update_on_duplicate used MagicMock without importing it`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
