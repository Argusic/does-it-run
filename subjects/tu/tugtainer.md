# tugtainer

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Quenary/tugtainer, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/tugtainer

## Pinned environment

- Project commit: `514f436c1ab3a0b2bf4da8068a15f73d856d0030`
- Test commit: `514f436c1ab3a0b2bf4da8068a15f73d856d0030`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 7.7 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8.5 | 4 | 4 | [run](https://argusic.com/run/d1c85b03-4774-4c6c-a512-d0018d4e1b00) |
| 2 | pass with mocks | 92 | 2 | 7.7 | 0 | 0 | [run](https://argusic.com/run/f52e47bb-46a1-4cc1-9177-711255b1bfbe) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Python 3.12 available but project requires >=3.13`
- 1 min: `'alembic' bare command not found in subprocess`
- 1 min: `Default DB_URL points to /tugtainer/tugtainer.db (unwritable)`
- 0.5 min: `AGENT_SECRET not set, auth would fail at runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
