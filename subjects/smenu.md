# smenu

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/p-gen/smenu, licensed MPL-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/smenu

## Pinned environment

- Project commit: `c8040ebffce01779854f5f105ff1bb8163db110e`
- Test commit: `c8040ebffce01779854f5f105ff1bb8163db110e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 9.3 to 19.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 9.3 | 0 | 0 | [run](https://argusic.com/run/133a3f34-f5d6-4e97-97dd-8e5d90e67255) |
| 2 | pass with mocks | 92 | 22 | 19.6 | 3 | 3 | [run](https://argusic.com/run/629f0ed2-b49e-4e56-92c8-27c963646aef) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `configure: unable to find tputs() in libtinfo/libncursesw (no .so linker symlinks)`
- 3 min: `make: fatal error: term.h: No such file or directory (ncurses dev headers missing)`
- 10 min: `Formal test suite (tests/*.sh) requires ptylie with root privileges for keystroke injection , setuid not effective in this container, ptylog is zero bytes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
