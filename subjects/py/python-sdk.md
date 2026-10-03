# python-sdk

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/modelcontextprotocol/python-sdk, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/python-sdk

## Pinned environment

- Project commit: `d060b36e1d095ef6e93e07ba5d59bb69b2ad449a`
- Test commit: `d060b36e1d095ef6e93e07ba5d59bb69b2ad449a`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 4.8 to 43.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.25 | 4.8 | 0 | 0 | [run](https://argusic.com/run/54891160-41ed-4b95-b8ae-dbb8d18cebb0) |
| 1 | pass | 100 | 0.03 | 43.3 | 1 | 1 | [run](https://argusic.com/run/15699571-da7c-4964-8c4b-d0f02fce310c) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `FreePortFactory in anyio pytest_plugin hangs when IPv6 loopback (::1) cannot bind but socket.has_ipv6 is True`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
