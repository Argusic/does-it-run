# yomikiru

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mienaiyami/yomikiru, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/yomikiru

## Pinned environment

- Project commit: `d0a86c5b5f17c452dd7f59a6f88917d987f39bad`
- Test commit: `d0a86c5b5f17c452dd7f59a6f88917d987f39bad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.7 to 6.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 6.7 | 4 | 4 | [run](https://argusic.com/run/41f3a37d-f864-422a-bc84-0537b0cddaf4) |

## What was observed on a clean machine

Attempt 1:

- `canvas native module fails: pixman-1 pkg-config not found`
- 0.5 min: `electron-winstaller not installed (optional dep of @electron-forge/maker-squirrel)`
- 0.3 min: `@biomejs/cli-linux-x64-musl missing (broken pnpm symlink)`
- 0.1 min: `Electron SUID sandbox requires root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
