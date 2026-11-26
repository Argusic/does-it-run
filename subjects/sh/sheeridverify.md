# sheeridVerify

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JenkinWoo/sheeridVerify, licensed ISC, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/sheeridverify

## Pinned environment

- Project commit: `bc7bf16d7a65e26c6e80b69d76526ee95e06794a`
- Test commit: `bc7bf16d7a65e26c6e80b69d76526ee95e06794a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 1.6 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 1.6 | 1 | 1 | [run](https://argusic.com/run/84d5ed10-479e-4e98-8a7b-759a9741d3ec) |
| 2 | pass | 100 | 4 | 4.5 | 2 | 2 | [run](https://argusic.com/run/efa00f33-57dd-4143-a1c2-116d0d666a9e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 below minimum requirement v22.15`

Attempt 2:

- 1 min: `System Node.js v18.19.1 below required v22.15`
- 1 min: `npm/npx binaries in Node.js tarball were 0-length files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
