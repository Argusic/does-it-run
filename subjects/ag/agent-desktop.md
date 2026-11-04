# agent-desktop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vercel-labs/agent-desktop, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/agent-desktop

## Pinned environment

- Project commit: `d3dc190afbf34cd2377252398ddd5c30efbd093a`
- Test commit: `d3dc190afbf34cd2377252398ddd5c30efbd093a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.9 to 61.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 12.9 | 3 | 3 | [run](https://argusic.com/run/377fd137-bbac-4242-80cb-7b2cf667b854) |
| 2 | pass | 100 | 28 | 61.8 | 8 | 8 | [run](https://argusic.com/run/798dd0bf-2755-4e5d-99a2-be7a1879300d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm install -g agent-desktop failed with EACCES because npm prefix /usr/local is owned by root`
- 2 min: `Rust toolchain was absent from PATH`
- 5 min: `Linux source build initially lacked AT-SPI/GTK session support, so accessibility commands returned PLATFORM_NOT_SUPPORTED`

Attempt 2:

- 2 min: `global npm prefix /usr/local not writable (EACCES)`
- 4 min: `no Rust toolchain in container`
- 6 min: `at-spi2-core daemons (at-spi-bus-launcher, at-spi2-registryd) not installed; no root`
- 20 min: `org.a11y.Bus activation blocked: /usr/share/defaults/at-spi2 and /etc and dbus service dirs unwritable, chroot/unshare denied`
- 15 min: `Linux E2E prereqs missing: gdbus, gsettings, fusermount, xdotool, wmctrl, xclip, openbox, PyGObject`
- 5 min: `GSettings a11y schemas missing from system gschemas.compiled`
- 3 min: `openbox exited: theme and menu not found`
- 3 min: `no live WM on shared Xvfb :99, stale NET_SUPPORTING_WM_CHECK`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
