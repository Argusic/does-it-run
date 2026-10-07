# mcpvault

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bitbonsai/mcpvault, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mcpvault

## Pinned environment

- Project commit: `c5abeda9bed11864079f70ae7f33d134e294aad2`
- Test commit: `c5abeda9bed11864079f70ae7f33d134e294aad2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 4.1 | 1 | 1 | [run](https://argusic.com/run/1409e01c-40c2-4736-932d-ad1101fff9e0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 is below required v20.0.0 , vitest crashes with 'node:util' missing export`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
