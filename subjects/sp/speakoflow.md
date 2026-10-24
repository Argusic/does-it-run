# SpeakoFlow

**Verdict: not yet verified.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AbhishekBarali/SpeakoFlow, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/speakoflow

## Pinned environment

- Project commit: `d6321032f35230f6e185f19812264ec2c8e206ee`
- Test commit: `d6321032f35230f6e185f19812264ec2c8e206ee`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 25.1 to 25.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 24 | 25.1 | 1 | 1 | [run](https://argusic.com/run/1da35e8f-9347-45aa-aa27-4438e5f8fb42) |

## What was observed on a clean machine

Attempt 1:

- 24 min: `bun install frontend succeeded but Rust/Tauri backend build fails: missing ~70 system -dev packages (libgtk-3-dev, libwebkit2gtk-4.1-dev, libpipewire-0.3-dev, libvulkan-dev, libclang-18-dev, etc.) requiring root to install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
