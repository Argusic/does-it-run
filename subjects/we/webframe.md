# webframe

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tractordev/webframe, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/webframe

## Pinned environment

- Project commit: `25c24cb61aadbce8f23cf46e6dd09abaad4d2143`
- Test commit: `25c24cb61aadbce8f23cf46e6dd09abaad4d2143`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19 to 19 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 19 | 5 | 5 | [run](https://argusic.com/run/f4af2226-a9fe-4607-b1ff-6417910e896f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed in container`
- 4 min: `WebKitGTK 6.0 shared libraries not found on system`
- 5 min: `WebKitGTK 6.0 requires bubblewrap sandbox which fails (no user namespaces)`
- 5 min: `4.1 subprocess binaries not found at hardcoded /usr/lib path`
- 2 min: `Missing dbus-launch, xdg-dbus-proxy, bubblewrap`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
