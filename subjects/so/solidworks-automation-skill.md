# solidworks-automation-skill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wzyn20051216/solidworks-automation-skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/solidworks-automation-skill

## Pinned environment

- Project commit: `2719ed8a7a653d5c4c28ef30c0af0bffbdd44962`
- Test commit: `2719ed8a7a653d5c4c28ef30c0af0bffbdd44962`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.2 to 23.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 23.2 | 4 | 4 | [run](https://argusic.com/run/ad3d89bd-02dc-4c66-a05e-b9793274e4ea) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `scripts package import triggers interactive COM dependency prompt on Linux, causing OSError and 44 collection errors`
- 1 min: `acad_dotnet_preflight.py uses Path().name which cannot parse Windows backslash paths on Linux`
- 2 min: `cad_installation.py resolve_shortcut_target and _common_candidates mishandle Windows paths on Linux`
- 1 min: `Desktop app fails on xcb platform because libxcb-cursor0 system library is missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
