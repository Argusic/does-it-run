# claude-plugins-official

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/anthropics/claude-plugins-official, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-plugins-official

## Pinned environment

- Project commit: `58267944f92187b7d6a1c822165c96c81c864806`
- Test commit: `58267944f92187b7d6a1c822165c96c81c864806`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.1 to 59.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 59.2 | 0 | 0 | [run](https://argusic.com/run/c25ed6fd-b8a8-4fd9-b1b6-05a32ee6ae22) |
| 2 | pass | 100 | 6 | 6.1 | 3 | 3 | [run](https://argusic.com/run/2507681f-4658-488e-bfc8-f0721402cbc5) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `4 agent .md files had YAML frontmatter parse failures because validate-frontmatter.ts's quoteSpecialValues() treated '|' (a YAML block scalar indicator) as a special character needing quoting, producing invalid YAML`
- 1 min: `npm install -g failed with EACCES (no root permissions)`
- 1 min: `bun not pre-installed in the container; required for MCP server TypeScript files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
