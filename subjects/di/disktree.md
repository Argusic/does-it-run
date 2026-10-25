# disktree

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tobi/disktree, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/disktree

## Pinned environment

- Project commit: `9b18b272ca3c5a145f6ff58eaf89dc4d311eeaea`
- Test commit: `9b18b272ca3c5a145f6ff58eaf89dc4d311eeaea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.1 to 21.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 21.1 | 4 | 4 | [run](https://argusic.com/run/bf0ee8c5-42e0-4ba1-9661-5f6d7384699b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Rust toolchain missing`
- 3 min: `yeslogic-fontconfig-sys build fails: fontconfig.pc not in pkg-config`
- 2 min: `Linker missing libxcb, libxkbcommon, libxkbcommon-x11 unversioned .so symlinks`
- 1 min: `Portable build fails without musl cross-compilation targets`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
