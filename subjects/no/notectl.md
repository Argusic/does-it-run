# notectl

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Samyssmile/notectl, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/notectl

## Pinned environment

- Project commit: `26a11a2e25691fa5c39bccd3a915fce4927d9c5a`
- Test commit: `26a11a2e25691fa5c39bccd3a915fce4927d9c5a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 1 | 4.1 | 4 | 3 | [run](https://argusic.com/run/5e783ca9-0815-4ba5-b6b1-318e2a073d8f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not installed in container`
- 2 min: `Node.js 18 missing styleText from node:util (rolldown dep)`
- 1 min: `Node 22.11.0 too old for Vite/Astro (need 22.12+)`
- `examples-angular build fails: needs Node 22.22.3+`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
