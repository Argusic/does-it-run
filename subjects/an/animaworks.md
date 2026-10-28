# animaworks

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xuiltul/animaworks, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/animaworks

## Pinned environment

- Project commit: `f700ff9a8311a3813be450da93875ed48c29eb50`
- Test commit: `f700ff9a8311a3813be450da93875ed48c29eb50`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 43.9 to 43.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 43.9 | 5 | 5 | [run](https://argusic.com/run/0ee8b82e-dcbf-477e-b0ea-de6ef0d3f6a7) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `IPv4-mapped IPv6 loopback addresses (::ffff:127.0.0.1) not detected as localhost`
- 4 min: `zstd CLI binary not available; scripts/cleanup_runtime.py could not create archives`
- 3 min: `Node.js 18 cannot load .js files as ESM without 'type': 'module' in package.json`
- 2 min: `crypto.randomUUID() not defined in Node 18 ESM mode (test_thread_logic_lifecycle)`
- 2 min: `3 test files needed adaptation to match fixes above`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
