# pgmoneta

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pgmoneta/pgmoneta, licensed BSD-3-Clause, written in C.

Evidence and recordings: https://argusic.com/subject/pgmoneta

## Pinned environment

- Project commit: `be594e442ee6dac3d76a97ee5ea8ee941bccbd83`
- Test commit: `be594e442ee6dac3d76a97ee5ea8ee941bccbd83`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28 to 28 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 28 | 5 | 5 | [run](https://argusic.com/run/041c80a5-f3fb-468a-93bd-1e27028c65fc) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing -dev packages (libev-dev, liblz4-dev, libzstd-dev, libbz2-dev, libarchive-dev, libssh-dev, libyaml-dev, ncurses-dev)`
- 3 min: `Missing rst2man/docutils for man page generation`
- 1 min: `libev header triggers GCC strict-aliasing -Werror failures`
- 3 min: `ncurses linker script fails to resolve libncurses.so.6 and -ltinfo`
- 3 min: `COLOR_* macro conflict between utils.h (ANSI strings) and ncurses.h (integer constants) in walinfo.c`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
