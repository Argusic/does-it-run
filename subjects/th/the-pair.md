# the-pair

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/timwuhaotian/the-pair, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/the-pair

## Pinned environment

- Project commit: `332bc2be80d5697538550efc1fcc359e466497a7`
- Test commit: `332bc2be80d5697538550efc1fcc359e466497a7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 51.1 to 51.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 50 | 51.1 | 5 | 5 | [run](https://argusic.com/run/15529f3f-ae04-49a2-8446-2b65dfd4fb25) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 installed but project requires >=22.22`
- 10 min: `Rust toolchain not found`
- 30 min: `Missing Tauri system libraries (libwebkit2gtk-4.1-dev, libgtk-3-dev, ~50 other -dev packages)`
- 3 min: `Static .a libraries in sysroot caused lld to prefer them over shared libs, producing undefined symbol errors`
- `1 of 10 headless e2e tests fails (command palette Cmd+K key shortcut not detected in headless Chrome)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
