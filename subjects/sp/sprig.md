# sprig

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hackclub/sprig, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/sprig

## Pinned environment

- Project commit: `7c32a85a62a5950af4e45cc29a9e4f2808fa7fa8`
- Test commit: `7c32a85a62a5950af4e45cc29a9e4f2808fa7fa8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.9 to 14.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 6.9 | 0 | 0 | [run](https://argusic.com/run/17a03eec-1abf-41b4-be12-032fd38f5aeb) |
| 2 | pass | 100 | 14 | 14.9 | 5 | 5 | [run](https://argusic.com/run/fa1fbed5-d7b7-437b-9e51-fce89ed3cb26) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Bun not installed (no unzip available); used npm instead`
- 1 min: `npm peer-dep conflict on Node 18 (Cannot read properties of null reading edgesOut)`
- 1 min: `Node 18 unsupported by Astro 6 (requires >=22.12.0)`
- `EMILE too many open files when watching (ulimit too low)`
- `Missing react dependency for react-icons`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
