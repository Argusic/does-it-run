# CowAgent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zhayujie/CowAgent, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/cowagent

## Pinned environment

- Project commit: `4ea7bdb452553392e7b29c7d55467a53ebc049e6`
- Test commit: `4ea7bdb452553392e7b29c7d55467a53ebc049e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.3 to 17.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 5.3 | 1 | 1 | [run](https://argusic.com/run/83ac5dec-c23b-4793-9cf3-4fd590b75fd6) |
| 2 | pass | 100 | 3 | 17.4 | 1 | 1 | [run](https://argusic.com/run/54fe2a29-b76c-4320-8cba-05f717080a87) |

## What was observed on a clean machine

Attempt 1:

- `test_a_zombie_does_not_count_as_alive fails in full suite (os.fork() in multi-threaded pytest-asyncio context)`

Attempt 2:

- 5 min: `test_a_zombie_does_not_count_as_alive failed in full suite (zombie detection race with multi-threaded fork)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
