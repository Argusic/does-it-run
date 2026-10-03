# ublacklist

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iorate/ublacklist, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ublacklist

## Pinned environment

- Project commit: `c395a019443bd2a1a842ac84fc697298cfd356f0`
- Test commit: `c395a019443bd2a1a842ac84fc697298cfd356f0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.2 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 2.2 | 2 | 2 | [run](https://argusic.com/run/2f218883-155f-4688-81a7-da350ebd185c) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pnpm not found in PATH , needed npm install -g to user prefix`
- 3 min: `Build failed: builtin/ submodule empty , 10 esbuild resolution errors for #builtin/serpinfo/*.yml imports`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
