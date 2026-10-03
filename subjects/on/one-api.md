# one-api

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/songquanpeng/one-api, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/one-api

## Pinned environment

- Project commit: `8df4a2670b98266bd287c698243fff327d9748cf`
- Test commit: `8df4a2670b98266bd287c698243fff327d9748cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.3 to 16.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 16.3 | 2 | 2 | [run](https://argusic.com/run/22299b28-8451-4c87-8d4f-37d96c4c718d) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Test images from Wikimedia Commons returned HTTP 400/429 instead of valid images`
- 3 min: `Handmade GIF and 1x1 JPEG test images had invalid LZW encoding / short Huffman data`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
