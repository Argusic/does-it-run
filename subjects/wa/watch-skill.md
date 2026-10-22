# watch-skill

**Verdict: could not verify.** Not scored (no completed run has a score).

Project: https://github.com/oxbshw/watch-skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/watch-skill

## Pinned environment

- Project commit: `f1317c8fe64744a606c31867b05fbbe3144268c6`
- Test commit: `f1317c8fe64744a606c31867b05fbbe3144268c6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 88 to 94.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 3 | 94.9 | 3 | 2 | [run](https://argusic.com/run/4b9ef520-696b-4ede-a337-f168ad43bf87) |
| 2 | timeout | none | 1.8 | 88 | 3 | 3 | [run](https://argusic.com/run/08570fa3-6aa3-4cf1-ac88-4afc2d7377c5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Playwright browser binaries not installed after 'uv sync'`
- `ONNX Runtime pthread_setaffinity_np failures on this container (192 vCPUs, affinity mask mismatch) cause some test files to hang indefinitely`
- `test_surfaces/test_cli_markup.py::test_a_status_is_still_coloured fails - ANSI escape codes not emitted in StringIO capture`

Attempt 2:

- 0.5 min: `'python' binary not found on PATH (only 'python3' exists)`
- 1 min: `NO_COLOR=1 and TERM=dumb in container suppress Rich ANSI output`
- 0.2 min: `Playwright Chromium browser not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
