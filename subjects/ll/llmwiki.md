# llmwiki

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lucasastorian/llmwiki, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/llmwiki

## Pinned environment

- Project commit: `aac3e6493306b7fff3b09cb181ca93918e93d0e6`
- Test commit: `aac3e6493306b7fff3b09cb181ca93918e93d0e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.8 to 17.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 17.6 | 0 | 0 | [run](https://argusic.com/run/ac06244a-e4bb-44a9-b266-54499759fdea) |
| 2 | pass | 100 | 15.5 | 15.8 | 3 | 3 | [run](https://argusic.com/run/b8f0995c-6c42-4165-9cc8-98a64e68af6f) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `mcp/services/__init__.py (empty file) made mcp/services a regular package, shadowing api/services when both dirs were on sys.path, causing 14 test collection errors`
- 3.5 min: `SQLite schema in api/infra/db/sqlite.py referenced non-existent column knowledge_base_id in documents table, causing 500 error on POST note`
- 3 min: `Web app requires Node.js >=20.9.0, but system had v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
