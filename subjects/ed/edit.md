# edit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/edit, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/edit

## Pinned environment

- Project commit: `c470ca59af44c176ea39c672d09b32061c274896`
- Test commit: `c470ca59af44c176ea39c672d09b32061c274896`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.3 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 7.1 | 1 | 1 | [run](https://argusic.com/run/3a49fcde-34bc-49e0-be70-779acf44e8a9) |
| 2 | pass | 100 | 0.5 | 6.3 | 2 | 2 | [run](https://argusic.com/run/b8754090-2594-46c2-817c-d7ee391b6890) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `ICU library on Ubuntu 24.04 uses versioned exports (u_errorName_74) and versioned .so filenames (libicuuc.so.74), but the project defaults to unversioned names (libicuuc.so) and unversioned symbols (u_errorName). Two tests (replace_one_zero`

Attempt 2:

- 8 min: `ICU library defaults don't match Ubuntu 24.04 packaging (libicuuc.so.74 with versioned symbols). Only libicuuc.so.74 symlink exists, no libicuuc.so. Also ICU on this system uses versioned symbols (u_errorName_74), not bare symbols (u_errorN`
- 5 min: `ICU auto-detect not usable because the default SONAME (libicuuc.so) doesn't exist; and when SONAME is overridden, the build script logic disables auto-detect because SONAME env var is non-empty, so the version suffix must be provided manual`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
