# homeassistant-blitzortung

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mrk-its/homeassistant-blitzortung, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/homeassistant-blitzortung

## Pinned environment

- Project commit: `2c3b4a35438c616259ad943ee8bfd3eee56deb87`
- Test commit: `2c3b4a35438c616259ad943ee8bfd3eee56deb87`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 34.4 to 34.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 32 | 34.4 | 3 | 2 | [run](https://argusic.com/run/2e1ef791-74a1-417a-be7b-b4887f002482) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Container only had Python 3.12 but requirements need 3.13/3.14; initial pip install failed for pytest-homeassistant-custom-component==0.13.366`
- 5 min: `ws-client crashed on Python 3.14: asyncio.get_event_loop() with no running loop raises RuntimeError`
- 45 min: `Upstream blitzortung websocket stream: ws-client's LZW decoder cannot decode current server frames (ws3/ws7 return HTTP 502; ws1/ws8 serve frames in an encoding the pinned client code doesn't parse); also blitzortung.ha.sed.pl:1883 closes T`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
