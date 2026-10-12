# GhidraMCP

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LaurieWired/GhidraMCP, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/ghidramcp

## Pinned environment

- Project commit: `1e980252087b2479a21b9ca6d82d5829538651a7`
- Test commit: `1e980252087b2479a21b9ca6d82d5829538651a7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 4.7 to 4.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 3 | 4.7 | 2 | 1 | [run](https://argusic.com/run/dc45319c-337f-4a8e-8502-9041320fb93e) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `pytest not installed in venv (uv absent; README's pip path used instead)`
- 30 min: `23 tests skipped: headless integration suite requires GHIDRA_INSTALL_DIR (Ghidra 12.1.4), the built extension jar, and Java 21, none of which exist in the container and no root to install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
