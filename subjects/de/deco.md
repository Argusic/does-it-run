# deco

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deco-cx/deco, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/deco

## Pinned environment

- Project commit: `7dbb79ae257338630ffbe41ab44c953fb86ab845`
- Test commit: `7dbb79ae257338630ffbe41ab44c953fb86ab845`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 5.9 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 16.1 | 3 | 3 | [run](https://argusic.com/run/29493b8e-bc0d-4cf2-aa70-dcb479fe012a) |
| 2 | pass | 100 | 6 | 5.9 | 2 | 2 | [run](https://argusic.com/run/4ba3f551-dc8d-445b-b4ce-2ea9a6521ddf) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Deno runtime in container; 'deno' not found and install.sh needed unzip`
- 3 min: `Project scripts/dev.ts is a linker (rewrites import maps), not a site dev server; daemon deploy-side manifest 'bundleApp' needs a non-GitHub-importable preact/jsx-runtime mapping that worked in the mock`
- 2 min: `Deno.watchFs (and inotify_init at libc level) fails with EMFILE errno 24 for every process, including a fresh python3, while fs.file-nr=53982/5000000 and ulimit=524288`

Attempt 2:

- 1 min: `Deno binary not found in PATH`
- 0.5 min: `Daemon fails on default port 8000 (EADDRINUSE)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
