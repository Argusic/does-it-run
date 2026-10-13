# free-ai-tools

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ShaikhWarsi/free-ai-tools, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/free-ai-tools

## Pinned environment

- Project commit: `8f802d7a76e4ac70dd490aca5f0473937e32cbd2`
- Test commit: `8f802d7a76e4ac70dd490aca5f0473937e32cbd2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.1 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 7 | 3.1 | 3 | 2 | [run](https://argusic.com/run/4fbd5763-fef2-4a36-9d16-d5d03e7a8508) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Container Node v18.19.1 is below the Node >=20.9 requirement of next@16.2.3`
- 1 min: `Backgrounded 'next start' was killed when its parent shell exited`
- `npm run lint exits nonzero with 6 pre-existing errors (React hooks order, unescaped entities, require() in tailwind.config.ts) and 20 warnings`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
