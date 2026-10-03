# skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/davidondrej/skills, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/run/d29fc2ca-924b-4c33-aaa7-e1b7f9112c73

## Pinned environment

- Project commit: `a10738f076bedf4683573f896d8dc814f13d3b04`
- Test commit: `a10738f076bedf4683573f896d8dc814f13d3b04`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 14 | 4 | 4 | [run](https://argusic.com/run/d29fc2ca-924b-4c33-aaa7-e1b7f9112c73) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `dangerous-patterns.txt missing - the guard script (~/.agents/hooks/deny-dangerous.sh) references ~/.agents/hooks/dangerous-patterns.txt but the file did not exist`
- 1 min: `~/.agents/ directory did not exist - the guard scripts reference ~/.agents/hooks/ but the directory was not present`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
