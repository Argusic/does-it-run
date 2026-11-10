# paperthin

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LilMGenius/paperthin, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/paperthin

## Pinned environment

- Project commit: `1306ea4a2c038b5dee508db23197b3a19ccfbdfc`
- Test commit: `1306ea4a2c038b5dee508db23197b3a19ccfbdfc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.2 to 16.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 16.2 | 3 | 3 | [run](https://argusic.com/run/2985c3d9-97ac-4de2-a6d8-9b27474785cb) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `ESM module loaded with require() in scripts/gates/prose.cjs crashes with ERR_REQUIRE_ESM`
- 2 min: `skills.test.cjs has stale SHA256 for Codes quick_validate.py`
- 3 min: `npm test glob pattern **/*.test.* not expanded by sh`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
