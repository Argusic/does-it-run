# VoxtMini

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hehehai/VoxtMini, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/voxtmini

## Pinned environment

- Project commit: `77751c892c6c8b1a777a0d2d36d23446d49928f3`
- Test commit: `77751c892c6c8b1a777a0d2d36d23446d49928f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 8.7 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 12.3 | 3 | 3 | [run](https://argusic.com/run/6d89b087-9ddf-4868-b86c-53512c8aff63) |
| 2 | pass with mocks | 92 | 9 | 8.7 | 2 | 2 | [run](https://argusic.com/run/498fed51-c5c1-4df8-8559-0d7cc7846773) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Go 1.27.4 installed in the container`
- 2 min: `Missing CJK font: TestOverlayInkMemoryNotice/zh-Hans and TestOverlayInk/live-short-zh and TestOverlayInk/live-long-zh failed with 'no font for Chinese'`
- `TestInfoTipCentred: zh-Hans '位置' label glyph centre 0.75 DIPs off from info icon (tolerance ±0.5 DIPs)`

Attempt 2:

- 1 min: `Go not found in container`
- 1 min: `TestInfoTipCentred failed for Chinese locale (no ink for zh-Hans text)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
