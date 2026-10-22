# claude-token-optimizer

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nadimtuhin/claude-token-optimizer, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/claude-token-optimizer

## Pinned environment

- Project commit: `a1e437a8c29909fd2db56d253cee7ef518ecfa47`
- Test commit: `a1e437a8c29909fd2db56d253cee7ef518ecfa47`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.7 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 7.7 | 3 | 3 | [run](https://argusic.com/run/b502153d-f01b-43f2-989b-66094f011897) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node 18 installed but project requires Node 20+`
- `chalk@6.0.0 and commander@15.0.0 require Node >=22, only Node 20 available; EBADENGINE warnings but packages work`
- 3 min: `bc not available in container; 5 hook scripts silently fell back to 0/? token estimates, causing 1 test failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
