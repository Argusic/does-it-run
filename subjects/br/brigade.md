# brigade

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/spinabot/brigade, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/brigade

## Pinned environment

- Project commit: `4c2a18fba9a7224fbddd07557ad3933866f60495`
- Test commit: `4c2a18fba9a7224fbddd07557ad3933866f60495`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 46.7 to 46.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 46.7 | 3 | 3 | [run](https://argusic.com/run/064473dd-3e86-4e0c-86b2-21203a03340f) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `System Node.js v18.19.1 , Brigade requires >=22.12`
- 0.5 min: `TypeScript compiler heap OOM (1GB default) during npm run build and npm test typecheck step`
- `MCP e2e test (mcp-cmd.e2e.test.ts) spawnSync ETIMEDOUT , the test spawns a child node process with tsx which hangs without a configured provider/model`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
