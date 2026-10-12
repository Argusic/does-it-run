# monolingual

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/reader-dict/monolingual, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/monolingual

## Pinned environment

- Project commit: `145d71595f3e62a0ad0445444e2c15e3a74cd5f4`
- Test commit: `145d71595f3e62a0ad0445444e2c15e3a74cd5f4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 70.9 to 70.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 60 | 70.9 | 10 | 10 | [run](https://argusic.com/run/7abf4bd8-ec75-4a21-8118-1ef9aad904b3) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `pip install failed on git submodule wikitextprocessor (hung on clone)`
- 2 min: `pyproject.toml filterwarnings pattern mismatched imghdr deprecation message`
- 3 min: `parse test fixture produced .xml.bz2 only, parse.main() needs .xml`
- 10 min: `Stale pre-built SQLite DB (5 rows, missing cacheable column) kept reverting`
- 5 min: `kindling binary missing at ~/.local/bin/kindling`
- 3 min: `_get_cache_exclusions() crashed with no such column: cacheable on fresh DBs`
- 2 min: `MOBI final_file is .mobi.zip but test expected .mobi`
- 2 min: `test_simple checked for .df file but DictFileFormat only produces .df.bz2`
- 2 min: `stardict-verify and stardict-bin2text missing from system`
- 1 min: `Count assertion in test_simple still checked for removed .df files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
