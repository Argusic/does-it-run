# text-to-cad

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/earthtojake/text-to-cad, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/text-to-cad

## Pinned environment

- Project commit: `4eaf7459a95c0547b089ab53aa579c7597fab1d5`
- Test commit: `4eaf7459a95c0547b089ab53aa579c7597fab1d5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 31.9 to 55.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 55.9 | 0 | 0 | [run](https://argusic.com/run/297af85c-3e1c-4b91-845a-a4ecd2a11122) |
| 2 | pass | 100 | 30 | 31.9 | 4 | 4 | [run](https://argusic.com/run/e7f2ea2b-8d6c-41c5-a36a-cef0514c891f) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `cadgen-js node_modules missing, causing 'three' import failure in tessellation cache cross-language test`
- `cadgen-js test suite requires Node 22, container has Node 18`
- `rsync missing , viewer client bundle step skipped in bundle.sh`
- 3 min: `pytest collection collision: multiple test files named test_cli.py and test_skill_structure.py across different skill test directories`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
