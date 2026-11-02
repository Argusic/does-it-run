# skill-conductor

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/smixs/skill-conductor, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/skill-conductor

## Pinned environment

- Project commit: `3c21d2f19c336d3a3333bfe4f45eee041bd13beb`
- Test commit: `3c21d2f19c336d3a3333bfe4f45eee041bd13beb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.6 to 5.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 5.6 | 2 | 2 | [run](https://argusic.com/run/1413e9bc-40ac-4cac-bf7f-3de0915b674d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `from scripts.utils import parse_skill_md fails under uv run , scripts/ is not a package`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
