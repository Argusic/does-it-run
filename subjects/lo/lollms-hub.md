# lollms_hub

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ParisNeo/lollms_hub, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/lollms-hub

## Pinned environment

- Project commit: `eb5a10676d7d0536b37d07220c9bf590fb2f74c9`
- Test commit: `eb5a10676d7d0536b37d07220c9bf590fb2f74c9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 40.5 to 40.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 40.5 | 5 | 5 | [run](https://argusic.com/run/9c25091d-e893-4935-9a63-30b79b969da1) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `run.sh hub installer froze waiting on TTY input (read blocks) and ./run.sh exited 126 because it lacked +x; it also tries sudo apt for missing cairo dev headers`
- 3 min: `Mock Ollama backend was unreachable from the hub because the hub bound its outbound connection to the Docker gateway 127.0.0.11 while my first mock listened only on 127.0.0.1`
- 5 min: `A DB-full API key owned by non-admin user 2 defaulted to NoneType user during streaming, crashing the proxy task; gunicorn default (non-setsid) invocations also kept dying ~40s after start in this container`
- 4 min: `Streaming returned only '{}' until the mock was upgraded to HTTP/1.1 chunked transfer; httpx then delivered chunks and the hub streamed them`
- 1 min: `The repo ships only dummy tests (tests/test_dummy.py: 3 assertions) and no test_api/test_core directories despite DEVELOPMENT.md describing them`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
