# QwenPaw

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agentscope-ai/QwenPaw, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/qwenpaw

## Pinned environment

- Project commit: `ce748971ea9c20e714cfc1ae1a13d82a535e1cda`
- Test commit: `ce748971ea9c20e714cfc1ae1a13d82a535e1cda`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.3 to 44.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 44.3 | 4 | 4 | [run](https://argusic.com/run/ea39da56-b35d-4e1d-9b2f-d287db541ab9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `'qwenpaw init --defaults' without --accept-security aborted because security confirmation requires interactive TTY`
- 3 min: `Frontend build (npm run build) hit Node.js OOM with default heap`
- 1 min: `pip install failed due to externally managed environment (PEP 668)`
- 1 min: `test_remote_download assertion failed: expected file mode 0o644 but umask 0002 produces 0o664`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
