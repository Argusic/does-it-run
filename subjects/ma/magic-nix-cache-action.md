# magic-nix-cache-action

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DeterminateSystems/magic-nix-cache-action, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/magic-nix-cache-action

## Pinned environment

- Project commit: `84c0677f58dcedf3b91f8223ce36a9ea5b3c84b7`
- Test commit: `84c0677f58dcedf3b91f8223ce36a9ea5b3c84b7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.6 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 6 | 7.8 | 1 | 1 | [run](https://argusic.com/run/8afded1f-db91-4cc8-bec9-fd7f9a2a2536) |
| 2 | fail | 80 | 1.2 | 5.6 | 0 | 0 | [run](https://argusic.com/run/b540a9da-30a3-4375-9011-80ea8ffcbc3a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node.js v18.19.1 is too old for dependency tree (got v15 uses ES2024 /v regex flag; ncc output also contains /v flag regexes)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
