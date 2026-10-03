# collabmd

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/andes90/collabmd, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/collabmd

## Pinned environment

- Project commit: `bf9ed645e3d31de947dbe084f0d8372f41aef39b`
- Test commit: `bf9ed645e3d31de947dbe084f0d8372f41aef39b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 7.5 | 2 | 2 | [run](https://argusic.com/run/dbef2678-ee10-4516-a030-c3c18881f68c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `git merge-tree --quiet flag not supported in git 2.43.0 (container git version)`
- 1 min: `Node.js v18 found in environment but project requires >=26`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
