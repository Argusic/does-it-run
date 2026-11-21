# heard

**Verdict: runs.** Argusic Score 89.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/heardlabs/heard, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/heard

## Pinned environment

- Project commit: `c82958d08a77ea99cf5a901c1e0280263d77ee81`
- Test commit: `c82958d08a77ea99cf5a901c1e0280263d77ee81`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 2.9 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 3 | 2.9 | 3 | 1 | [run](https://argusic.com/run/372775af-a780-4ef1-8550-743c9bbf9679) |
| 2 | pass with mocks | 92 | 12 | 7.3 | 4 | 4 | [run](https://argusic.com/run/f2da06d3-65d6-4480-a674-006fcb87dd26) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pyobjc-framework-* (macOS-only deps) failed to build on Linux - sw_vers not found`
- `test_muted.py::test_speak_drops_when_mic_active fails - afplay not available on Linux`
- `test_in_app_update.py::test_unzip_app_extracts_bundle fails - unzip not available on Linux`

Attempt 2:

- 4 min: `pyobjc-framework-Cocoa, WebKit, Quartz, ApplicationServices fail to build on Linux (require /usr/bin/sw_vers)`
- 2 min: `rumps (pyobjc dependency) can't install on Linux`
- 4 min: `test_unzip_app_extracts_bundle: /usr/bin/unzip not found`
- 2 min: `test_speak_drops_when_mic_active: afplay not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
