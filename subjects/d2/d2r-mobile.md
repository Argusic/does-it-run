# d2r-mobile

**Verdict: not yet verified.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jhaizhou-ops/d2r-mobile, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/d2r-mobile

## Pinned environment

- Project commit: `21cf97b91823111ead237858ea79929afacf71a5`
- Test commit: `21cf97b91823111ead237858ea79929afacf71a5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 1; wall time 7.3 to 7.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 15 | 7.3 | 6 | 6 | [run](https://argusic.com/run/121e3011-4adc-4ee3-945f-ae98f2689fd9) |

## What was observed on a clean machine

Attempt 1:

- `System is Linux x86_64, not Apple silicon macOS (required by setup.sh)`
- 5 min: `Python packages could not be installed system-wide (externally managed environment on Ubuntu 24.04)`
- 5 min: `Many C tests fail on Linux due to missing macOS-only headers (TargetConditionals.h, mach/mach.h, malloc/malloc.h, sys/clonefile.h, mach/mach_time.h)`
- 2 min: `dm_textbox_core.c has multi-line comment that triggers GCC -Werror=comment`
- `dm_rift.c uses macOS-specific st_mtimespec; fails on Linux which uses st_mtim`
- `Several Python tools (nso.py, x18.py, sweep.py, movie_cut.py etc.) require game files (main.bin etc.) which are not present`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
