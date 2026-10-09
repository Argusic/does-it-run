# skillsgate

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/skillsgate/skillsgate, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/skillsgate

## Pinned environment

- Project commit: `917098adf25113bcbc436344d80d6efe88d2b849`
- Test commit: `917098adf25113bcbc436344d80d6efe88d2b849`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.4 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.4 | 4 | 4 | [run](https://argusic.com/run/ba1ff1a1-1c8a-4863-9385-0b7f712ba7a1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Container had only Node 18.19.1; project requires Node 22+`
- 3 min: `react-router dev failed: 'React Router Vite plugin not found in Vite config' because CLI resolved node to system Node 18`
- 1 min: `Desktop 'npm run dev' aborted: Electron SUID sandbox helper not configured (container has no setuid chrome-sandbox)`
- 2 min: `node build/server/index.js cannot run the built web bundle under plain Node (Worker only)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
