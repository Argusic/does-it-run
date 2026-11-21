# claude-codex-settings

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fcakyon/claude-codex-settings, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-codex-settings

## Pinned environment

- Project commit: `8c25677efb55b473f7b0bbbb3658273ebc8eb993`
- Test commit: `8c25677efb55b473f7b0bbbb3658273ebc8eb993`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 3 | 3 | 3 | [run](https://argusic.com/run/b648739b-1df7-4085-973b-093f0c08acdb) |
| 2 | pass | 100 | 24 | 4.6 | 4 | 4 | [run](https://argusic.com/run/c24701a0-e9b1-4a6f-b475-ccf103478a33) |

## What was observed on a clean machine

Attempt 1:

- 0.7 min: `Missing python3 yaml module (validate_plugins.py requires pyyaml)`
- 6 min: `Node.js v18 too old for Astro v7 (requires >=22.12.0)`
- 1.5 min: `Rolldown native binding not found after Node.js upgrade`

Attempt 2:

- `zip command not available in container`
- `Node.js v18.19.1 too old for Astro site build (needs >=22.12.0)`
- 1 min: `polar sync had stale checkout on first run (empty master branch)`
- 2 min: `slides_test.py missing pdf2image and pdftoppm`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
