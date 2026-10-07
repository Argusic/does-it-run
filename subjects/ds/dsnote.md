# dsnote

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mkiol/dsnote, licensed MPL-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/dsnote

## Pinned environment

- Project commit: `6ec0a315b4915a92ff0a1de0bd75e3c3037fbd21`
- Test commit: `6ec0a315b4915a92ff0a1de0bd75e3c3037fbd21`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 7.8 to 48.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 7.8 | 0 | 0 | [run](https://argusic.com/run/6b4fd5c5-c8b9-4568-b3ec-bf6b72db95b6) |
| 2 | fail | 20 | 25 | 48.5 | 2 | 2 | [run](https://argusic.com/run/054930da-c76e-4af7-a52a-8a3a8d1ab628) |

## What was observed on a clean machine

Attempt 2:

- 30 min: `Qt6 development headers/libs not installed system-wide; extracted from .deb packages without root access`
- 40 min: `Full build fails at dsnote_lib: 18+ source files reference external C/C++ APIs from webrtc_vad, rnnoise, espeak-ng, piper, libarchive, xz, sam, rdrview, cld2, taglib, ssplitcpp, maddy, html2md, cpp-pinyin, google_pinyinim, april-asr, xdo, q`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
