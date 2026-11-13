# agent-hud-open

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jazzenchen/agent-hud-open, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/agent-hud-open

## Pinned environment

- Project commit: `c6d41101012aafb6d24cc9bfbc0043f66e551c0a`
- Test commit: `c6d41101012aafb6d24cc9bfbc0043f66e551c0a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.9 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 55 | 8.9 | 3 | 3 | [run](https://argusic.com/run/92c4dd1b-d28a-4e94-acea-c2723f06b4b1) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `libglib2.0-dev system package not installed ('glib-2.0.pc' not found by pkg-config), blocking desktop/Tauri build on Linux (cargo fails on glib-sys build dependency)`
- 5 min: `MCP host-tools tests fail 6/6 because 'bun' is not in PATH (spawnSync bun ENOENT)`
- 3 min: `'.ts' test files in packages cannot run on Node 18 (need Node 22+ for native --experimental-run-ts); 13 app tests and 1 engine-client test skipped`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
