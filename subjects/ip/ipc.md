# ipc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Flow-IPC/ipc, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/ipc

## Pinned environment

- Project commit: `31b5919daf724273b53f08d4d3fa78f672ea9903`
- Test commit: `31b5919daf724273b53f08d4d3fa78f672ea9903`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 55.3 to 55.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 52 | 55.3 | 5 | 5 | [run](https://argusic.com/run/9555fad2-23bf-4eaf-85bf-d1135952d92c) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Flow conanfile.py missing exports_sources and VERSION exports for Conan 2 compatibility`
- 6 min: `Conan 2 option 'ANY' not valid for freestring options; jemalloc.prefix option missing in ConanCenter recipe`
- 5 min: `OOM due to 192 parallel compile jobs in 8GB container`
- 3 min: `Jemalloc built by ConanCenter lacks je_ prefix, causing unresolved symbols`
- `Install to /usr/local requires root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
