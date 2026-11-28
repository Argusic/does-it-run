# encrypted-note

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nniiovoo/encrypted-note, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/encrypted-note

## Pinned environment

- Project commit: `db2ada3f5273dc0ea543809ad1fe16ff313943fd`
- Test commit: `db2ada3f5273dc0ea543809ad1fe16ff313943fd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.7 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7.5 | 7.7 | 2 | 2 | [run](https://argusic.com/run/e6836c33-fa36-44e7-bd92-684a3293c697) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Tauri GUI app (encrypted-note-app) cannot build on Linux: requires GTK3/WebKit2 system development packages (libgtk-3-dev, libwebkit2gtk-4.1-dev, etc.) which need root to install`
- `Vite 8.x requires Node >=20.19, container has 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
