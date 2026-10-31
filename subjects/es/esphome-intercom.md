# esphome-intercom

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/n-IA-hane/esphome-intercom, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/esphome-intercom

## Pinned environment

- Project commit: `79c860f9c609d2309947ca0031164127a02077bb`
- Test commit: `79c860f9c609d2309947ca0031164127a02077bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 81.5 to 81.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 8 | 81.5 | 8 | 6 | [run](https://argusic.com/run/61e7743c-bade-47c8-90fb-73d8a31a8ef4) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Coordinated sibling ESP component repos could not be created under root-owned /work (PermissionError)`
- 3 min: `test_esphome_upstream_alignment failed: a hard-coded sibling path was not a filesystem path`
- 12 min: `pytest-homeassistant-custom-component==0.13.365 needs Python >=3.14; container has 3.12 and no root`
- 6 min: `Fallback plugin 0.13.205 pins HA 2025.1.4, which lacks 2026 APIs and auto-disabled sockets, breaking test_conference`
- 8 min: `Node.js 18.19.1 loads the frontend .js ESM modules as CommonJS (Unexpected token 'export'; named export not found)`
- 2 min: `test_mixer_gain_runtime checksum mismatch because esp-audio-libs main was newer than the pinned revision`
- 8 min: `test_yaml_paths_contract asserted a literal ../../../../esphome-esp-video-camera/components that cannot exist under root-owned /work`
- 2 min: `test_dahua_audio_socket invite timeout under full-suite load`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
