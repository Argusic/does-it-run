# obsidian-llm-wiki

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GD4AI/obsidian-llm-wiki, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/obsidian-llm-wiki

## Pinned environment

- Project commit: `aa143903749bd19c4e954b1b1d885949ed45e8c2`
- Test commit: `aa143903749bd19c4e954b1b1d885949ed45e8c2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.1 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 6.1 | 3 | 3 | [run](https://argusic.com/run/d155fe6b-cdac-4606-9c02-aeeeac6c3144) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pnpm: not found , not installed in base image`
- 3 min: `Node v18.19.1 < project requirement >=22`
- 0.5 min: `stale prefix in .npmrc broke npm subcommands`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
