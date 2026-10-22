# streampipes

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/streampipes, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/streampipes

## Pinned environment

- Project commit: `16aa0fb3a65ddabe0268a378f68dfa2c85d3949e`
- Test commit: `16aa0fb3a65ddabe0268a378f68dfa2c85d3949e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 45 to 70.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 70.9 | 0 | 0 | [run](https://argusic.com/run/b020be4b-659b-4fa2-b39b-1e4d098e81d9) |
| 2 | pass | 100 | 43 | 45 | 5 | 5 | [run](https://argusic.com/run/d6c187a7-641b-446b-ba68-a0a2daa8b988) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `No JDK 25 or Maven installed; Java and Maven were absent`
- 4 min: `Bundled Node.js v18 was too old for Angular (minimum v22.22.3)`
- 5 min: `Backend JAR initialization failed: host 'couchdb' unresolvable (CouchDB service absent)`
- 3 min: `pip3 install poetry blocked by PEP 668 externally-managed environment`
- `UI lint reports 5 pre-existing unused-variable errors (ng lint app)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
