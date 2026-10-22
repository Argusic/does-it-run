# MusicBox

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/asxez/MusicBox, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/musicbox

## Pinned environment

- Project commit: `d28652e5dace34e56df4170670c0d30a3df0748e`
- Test commit: `d28652e5dace34e56df4170670c0d30a3df0748e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.2 to 17.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 17.2 | 7 | 7 | [run](https://argusic.com/run/a97e8ba3-5d57-41ae-93e5-c62630687b31) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Container Node.js v18.19.1 is below the project's required >=22`
- 3 min: `No Rust toolchain in container; native audio crate requires one`
- 2 min: `System pip install refused by PEP 668 (externally-managed-environment)`
- 1 min: `Electron aborted: SUID chrome-sandbox not setuid-root (no root in container)`
- 20 min: `npm run build:rs fails on Linux: wasapi 0.21/windows 0.62 are Windows-only; wasapi crate unconditionally imports Win32 COM types, so no feature set compiles on non-Windows (tried default-features=false and cargo [patch] wasapi/windows-futur`
- 8 min: `npm run build:python fails: PyInstaller and Nuitka both need system libpython3.12.so.1.0/python3-dev, absent and uninstallable without root`
- 2 min: `Headless container has no ALSA/PulseAudio//dev/snd, so audible WebAudio output could not be observed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
