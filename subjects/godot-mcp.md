# godot-mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Coding-Solo/godot-mcp, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/godot-mcp

## Pinned environment

- Project commit: `1209744fad78f3998f98c7394fd0f6ef50da5281`
- Test commit: `1209744fad78f3998f98c7394fd0f6ef50da5281`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.5 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 11.5 | 2 | 2 | [run](https://argusic.com/run/de560115-1373-4645-834b-8cc8d5bd0c5a) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `require('fs') call in ESM module causes runtime warning in get_project_info`
- `load_sprite tool fails with real Godot headless: image loader needs rendering context`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
