# gel

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/geldata/gel, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/gel

## Pinned environment

- Project commit: `85191063b4db8b87caf26499de40f8a9d90c8146`
- Test commit: `85191063b4db8b87caf26499de40f8a9d90c8146`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 24.6 to 81.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 64 | 24.6 | 5 | 5 | [run](https://argusic.com/run/f02a60b4-590c-4ae3-aa10-47583dcbbc6a) |
| 2 | pass with mocks | 92 | 18 | 81.5 | 9 | 9 | [run](https://argusic.com/run/f3c37938-d897-47d3-bf16-e26b1ae73ada) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No git tags in repo; buildmeta.get_version_from_scm fails with ValueError: max() iterable argument is empty`
- 2 min: `Git submodules (postgres, pgproto, libpg_query) not initialized; 'edb/server/pgproto/uuid.pyx' and other paths missing`
- 6 min: `Python.h and pyconfig.h not found (no python3.12-dev package); C extension compilation fails`
- 2 min: `protobuf-c/protobuf-c.h not found for libpg_query C extension`
- 12 min: `PostgreSQL build fails: ICU library not found, then readline, then flex not in PATH, then bison not propagated correctly`

Attempt 2:

- 1 min: `Rust compiler not found`
- 1 min: `no git tags for version detection`
- 3 min: `missing python3.12-dev headers`
- 2 min: `missing protobuf-c.h`
- 1 min: `missing git submodules`
- 5 min: `postgres configure fails`
- 0.5 min: `Rust not in PATH`
- 2 min: `missing _buildmeta.py`
- 1 min: `missing pg_config binary for tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
