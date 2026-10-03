# openshot-qt

**Verdict: runs.** Argusic Score 80.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenShot/openshot-qt, licensed NOASSERTION, written in Python.

Evidence and recordings: https://argusic.com/subject/openshot-qt

## Pinned environment

- Project commit: `d2737c461f577df4d516e5d4609af55f3ea16d54`
- Test commit: `d2737c461f577df4d516e5d4609af55f3ea16d54`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 26 to 35.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass with mocks | 92 | 25 | 26 | 6 | 6 | [run](https://argusic.com/run/e80f44c8-ee82-4ea3-a9e2-dd7217bed107) |
| 2 | pass | 100 | 34 | 34.4 | 4 | 4 | [run](https://argusic.com/run/6ac67596-a797-42e3-86ec-3722e33fe937) |
| 3 | fail | 50 | 35 | 35.4 | 8 | 8 | [run](https://argusic.com/run/f5e56ae0-0b2b-4d3e-a9db-ba681aeb9060) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `ModuleNotFoundError: No module named openshot (libopenshot C++ library)`
- 1 min: `ModuleNotFoundError: No module named requests`
- 1 min: `ModuleNotFoundError: No module named zmq/pyzmq`
- 5 min: `Missing mock methods: Point.__init__ signature, Keyframe.AddPoint, Clip.Position/End/Json, DummyReader.Json, EffectInfo.Json() classmethod, Timeline.SetCache/Open/Clear/SetJson etc.`
- 2 min: `PyQt6 xcb platform missing libxcb-cursor0 (not installable without root)`
- `41 test failures out of 520+ due to mock not computing exact same values as real libopenshot C++ library`

Attempt 2:

- 8 min: `libopenshot 0.3.2 from Ubuntu noble missing Clip.CreateReader, ScreenCaptureSettings, ScreenCaptureReader, ClipProcessingJobs APIs`
- 3 min: `PyQt6 ButtonRole enum comparison fails in style_message_box (role == QDialogButtonBox.YesRole returns False on PyQt6 despite same value)`
- 2 min: `libopenshot 0.3.2 does not support Clip().SetJson({"reader":...}).Open() - test assumed newer API`
- 3 min: `tabifiedDockWidgets() returns empty on offscreen/minimal Qt platform until QMainWindow.show() is called`

Attempt 3:

- 2 min: `No Qt binding (PyQt6/PySide6) available in base environment`
- 1 min: `Missing 'requests' module`
- 10 min: `Missing 'openshot' C extension (libopenshot) - requires root for apt install, Qt5-incompatible with PyQt6, not on PyPI`
- 1 min: `Missing 'pyzmq' module`
- 5 min: `Mock Clip.Position missing setter/getter callable pattern`
- 3 min: `PyQt6 enum identity differs from PyQt5 - 'role in (AcceptRole, YesRole)' fails even with same value`
- 2 min: `Mock EffectInfo.CreateEffect returned None, called .Id() on it`
- `Full GUI launch fails: timeline/mock interactions in event loop initialization`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
