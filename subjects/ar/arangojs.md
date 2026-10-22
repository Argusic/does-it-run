# arangojs

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/arangodb/arangojs, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/arangojs

## Pinned environment

- Project commit: `205344fdd4cd0489c3bf4d79f3f41e1d60690f50`
- Test commit: `205344fdd4cd0489c3bf4d79f3f41e1d60690f50`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.6 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 9.6 | 4 | 4 | [run](https://argusic.com/run/dcc54eed-adee-4ac8-a20b-1242e89e2cd1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js version 18 found, project requires >=20`
- 3 min: `Docker unavailable for ArangoDB test server`
- 1 min: `arangod --database.init-database requires interactive password prompt`
- 2 min: `ArangoDB background process died after shell exit`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
