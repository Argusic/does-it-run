# redux

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/reduxjs/redux, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/redux

## Pinned environment

- Project commit: `56abca4749921d68f40cda20afd2043af9751f72`
- Test commit: `56abca4749921d68f40cda20afd2043af9751f72`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 20.2 to 20.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 20.2 | 1 | 1 | [run](https://argusic.com/run/71d4189b-2601-4175-8f34-380857524476) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Node.js v18.19.1 system Node is too old for native optional dependencies (oxfmt, oxlint, rolldown all require >=20.19 or >=22.12); native binaries not downloaded by pnpm install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
