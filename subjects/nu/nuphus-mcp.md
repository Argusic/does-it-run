# nuphus-mcp

**Verdict: runs.** Argusic Score 86.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mrpulor-gh/nuphus-mcp, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/nuphus-mcp

## Pinned environment

- Project commit: `95b860860934a5dc2da18c4d907f07a0e2902032`
- Test commit: `95b860860934a5dc2da18c4d907f07a0e2902032`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.6 to 11.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 12 | 11.6 | 3 | 1 | [run](https://argusic.com/run/75ac074d-8632-4457-a103-aec87133996e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing libxdo.so.3 - prebuilt binary would not launch`
- 5 min: `Rust build from source fails - wayland-dev, pipewire-dev, libclang system headers not available`
- `desktop_windows_list returns 'Platform not supported' in headless Xvfb`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
