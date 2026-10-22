# sightline

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ni5arga/sightline, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/sightline

## Pinned environment

- Project commit: `1095b9275f830d43113a621a15b9f4a017d78665`
- Test commit: `1095b9275f830d43113a621a15b9f4a017d78665`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 3 to 12 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 3 | 0 | 0 | [run](https://argusic.com/run/e4f34964-be10-423b-9dc7-2f2a854b70ca) |
| 2 | pass | 100 | 18 | 12 | 3 | 3 | [run](https://argusic.com/run/5b047706-54b9-432a-b925-a4a515ad1637) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18.19.1 too old for Next.js 16 (requires >=20.9.0)`
- 1 min: `next.config.ts had unrecognized key reactCompiler (Next.js 16 feature)`
- 1 min: `eslint.config.mjs imported submodules not found in eslint-config-next v15`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
