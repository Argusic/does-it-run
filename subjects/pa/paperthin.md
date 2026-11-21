# paperthin

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LilMGenius/paperthin, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/paperthin

## Pinned environment

- Project commit: `1306ea4a2c038b5dee508db23197b3a19ccfbdfc`
- Test commit: `1306ea4a2c038b5dee508db23197b3a19ccfbdfc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.7 to 16.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 16.2 | 3 | 3 | [run](https://argusic.com/run/2985c3d9-97ac-4de2-a6d8-9b27474785cb) |
| 2 | pass | 92 | 0.3 | 11.7 | 5 | 3 | [run](https://argusic.com/run/1f5cf382-74b4-483c-8b61-ce5e5817c2ca) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `ESM module loaded with require() in scripts/gates/prose.cjs crashes with ERR_REQUIRE_ESM`
- 2 min: `skills.test.cjs has stale SHA256 for Codes quick_validate.py`
- 3 min: `npm test glob pattern **/*.test.* not expanded by sh`

Attempt 2:

- 5 min: `prose.cjs uses require() to load ESM module find.mjs - fails on Node 18`
- 10 min: `restart-handoff.mjs uses fs.globSync which requires Node 22+`
- 1 min: `npm test command uses --test globs not supported in Node 18`
- `npx resolves to npx-cli.js symlink rather than through /usr/bin/node - container-specific layout`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
