# skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/qdrant/skills, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/run/a1c38d68-95b5-4356-ad11-5ba54b184698

## Pinned environment

- Project commit: `6a03d0ce8f554a579c2e14a81fb7e2245a708db0`
- Test commit: `6a03d0ce8f554a579c2e14a81fb7e2245a708db0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.5 to 2.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 2.5 | 2 | 2 | [run](https://argusic.com/run/a1c38d68-95b5-4356-ad11-5ba54b184698) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `sh rejected bash-ism ${PIPESTATUS} in my unittest wrapper`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
