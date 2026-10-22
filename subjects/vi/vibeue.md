# VibeUE

**Verdict: not yet verified.** Argusic Score 0 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kevinpbuckley/VibeUE, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/vibeue

## Pinned environment

- Project commit: `a231dcb57f22958ccb5207d9588dd357f2921f0d`
- Test commit: `a231dcb57f22958ccb5207d9588dd357f2921f0d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 1; wall time 9.1 to 9.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 0.4 | 9.1 | 1 | 0 | [run](https://argusic.com/run/43ecfe69-74c5-433f-a462-c437a88a0f1f) |

## What was observed on a clean machine

Attempt 1:

- 0.4 min: `No Unreal Engine 5.8+ installed in container. UE_ENGINE_ROOT is not set, no editor binary or UnrealBuildTool found. VibeUE requires the full UE 5.8 SDK to compile its C++ source and needs UE's embedded Python to run its Python scripts.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
