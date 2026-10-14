# Librian

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RimoChan/Librian, licensed MPL-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/librian

## Pinned environment

- Project commit: `4c8fd41687936c9bc80ed6a00aa57239e243c1ab`
- Test commit: `4c8fd41687936c9bc80ed6a00aa57239e243c1ab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.2 to 17.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 17.2 | 7 | 7 | [run](https://argusic.com/run/7cb80a9f-e3bc-4c9b-9fa3-5f00abfacae1) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pip install -e . failed due to externally-managed-environment (PEP 668)`
- 1 min: `FileNotFoundError: project template 潘大爺的模板 didn't exist`
- 1 min: `test path resolution: 根 = ../../ resolved to /work/ instead of /work/repo/`
- 1 min: `KeyError: '默認立繪位置' in 鏡頭.py`
- 2 min: `liber parser treated BGM/BG commands as 旁白 instead of 函數調用`
- 5 min: `test_port: listen-mode crashed on Qt WebEngine init (no dbus/X)`
- 2 min: `test_port: ConnectionRefused due to stale port 8000`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
