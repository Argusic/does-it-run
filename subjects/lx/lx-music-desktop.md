# lx-music-desktop

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lyswhut/lx-music-desktop, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/lx-music-desktop

## Pinned environment

- Project commit: `9c364b482e5621a1d38b50e8610d2fb974457e6e`
- Test commit: `9c364b482e5621a1d38b50e8610d2fb974457e6e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 3; wall time 10.5 to 17.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 10 | 10.5 | 2 | 2 | [run](https://argusic.com/run/e1cb1621-bc07-41f1-b2ff-2a5a3d897c1c) |
| 2 | fail | 80 | 12 | 13.3 | 4 | 4 | [run](https://argusic.com/run/36a7a5ed-77c3-4811-aef5-747872499d30) |
| 3 | fail | 80 | 15 | 17.5 | 6 | 6 | [run](https://argusic.com/run/03cff48b-b46d-4565-b7ad-92ee032156ed) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 is installed but project requires >=22 (electron 40, node 22)`
- 0.5 min: `Electron SUID sandbox helper not configured in container (chrome-sandbox not owned by root mode 4755)`

Attempt 2:

- 3 min: `System Node.js v18.19.1 did not meet requirement of Node.js >=22`
- 1 min: `First Electron launch failed with SQLITE_CANTOPEN 'unable to open database file'`
- `dbus errors: Failed to connect to socket /run/dbus/system_bus_socket (no dbus daemon in container)`
- `ALSA errors: no audio hardware in container`

Attempt 3:

- 3 min: `Node v18.19.1 too old (requires >=22)`
- 1 min: `npm install failed: Invalid comparator 'latest'`
- 1 min: `Build failed: missing eslint-plugin-import`
- 1 min: `Build failed: missing eslint-plugin-n and eslint-plugin-promise`
- 1 min: `Electron SUID sandbox incorrectly configured`
- 5 min: `App crashed with SIGABRT on headless Linux: use-gl=desktop not supported by headless Xvfb`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
