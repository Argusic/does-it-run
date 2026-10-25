# wireguard-gui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/0xle0ne/wireguard-gui, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/wireguard-gui

## Pinned environment

- Project commit: `43073da32ea217412971dcf4b288df800773e6d7`
- Test commit: `43073da32ea217412971dcf4b288df800773e6d7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 33.3 to 33.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 33.3 | 8 | 8 | [run](https://argusic.com/run/52bc2f99-f968-467d-9819-23b2ea4e6e5b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 is too old for Next.js 16 (requires >=20.9.0); next-build immediately failed`
- 1 min: `@tailwindcss/oxide native binary for x64-linux-gnu not installed , npm install with old Node.js didn't pull optional dependency`
- 10 min: `Missing system -dev packages (libglib2.0-dev, libgtk-3-dev, libwebkit2gtk-4.1-dev, etc.) , no root for apt-get install`
- 3 min: `Transitive pkg-config dependencies (xproto, kbproto, libffi, dbus-1, etc.) still missing from extracted .pc files`
- 3 min: `Linker picked up static .a archives (libgio-2.0.a, etc.) from dev packages instead of shared .so, causing missing symbols (mnt_*, dbus_*)`
- 5 min: `WebKit child processes (WebKitNetworkProcess, injected-bundle) hardcoded to /usr/lib/x86_64-linux-gnu/webkit2gtk-4.1/ , cannot create directory without root`
- 3 min: `Missing runtime libraries: libxslt, libgst*, libayatana-indicator, libdbusmenu, libdw, liborc`
- 1 min: `No dbus session bus , app printed warnings but continued`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
