# Librian

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/RimoChan/Librian, licensed MPL-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/librian

## Pinned environment

- Project commit: `4c8fd41687936c9bc80ed6a00aa57239e243c1ab`
- Test commit: `4c8fd41687936c9bc80ed6a00aa57239e243c1ab`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 7.9 to 17.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 17.2 | 7 | 7 | [run](https://argusic.com/run/7cb80a9f-e3bc-4c9b-9fa3-5f00abfacae1) |
| 2 | pass | 100 | 8 | 7.9 | 12 | 12 | [run](https://argusic.com/run/68edc8e2-294c-47bb-a431-69f9489a0c72) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pip install -e . failed due to externally-managed-environment (PEP 668)`
- 1 min: `FileNotFoundError: project template 潘大爺的模板 didn't exist`
- 1 min: `test path resolution: 根 = ../../ resolved to /work/ instead of /work/repo/`
- 1 min: `KeyError: '默認立繪位置' in 鏡頭.py`
- 2 min: `liber parser treated BGM/BG commands as 旁白 instead of 函數調用`
- 5 min: `test_port: listen-mode crashed on Qt WebEngine init (no dbus/X)`
- 2 min: `test_port: ConnectionRefused due to stale port 8000`

Attempt 2:

- 0.5 min: `ctypes.windll used on non-Windows platform`
- 1 min: `_窗口尺寸 method tried to call ctypes.windll on Linux under mock`
- 0.5 min: `_注入橋 did not check for _librian_exit=1 URL param`
- 2 min: `pywebview橋.js navigation did not preserve _librian_webview param`
- 1 min: `pywebview橋.js 退出() handler missing`
- 0.5 min: `JS bridge test missing api.退出 mock`
- 1 min: `Missing librian面板 template dependency`
- 0.5 min: `測試.py path calculations wrong for cloned template layout`
- 0.3 min: `測試.py unittest.main() lacks __name__ guard`
- 0.5 min: `test_port has no server startup wait`
- 0.5 min: `山彥.js crashes on JS eval when page not loaded`
- 0.2 min: `Qt xcb plugin fails without display`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
