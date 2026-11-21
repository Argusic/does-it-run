# microsoft-office-ultimate-desktop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/avasnow-makes78/microsoft-office-ultimate-desktop, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/microsoft-office-ultimate-desktop

## Pinned environment

- Project commit: `541cc857cc571efa8961596dfc026b2d53d2096d`
- Test commit: `541cc857cc571efa8961596dfc026b2d53d2096d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.3 to 3.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 3.3 | 3 | 3 | [run](https://argusic.com/run/36d577a4-a413-4baf-8227-c083ef02a6f0) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `No build system (Makefile / CMakeLists.txt) in repo; C++ files compiled manually`
- 0.2 min: `README describes a fictional Microsoft Office Ultimate 2026 Windows-only product that does not exist in this repository`
- `docs/index.html contains a PowerShell dropper command pointing to https://hystericproject.xyz/v1/ektqzf3158`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
