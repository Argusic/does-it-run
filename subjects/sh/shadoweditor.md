# ShadowEditor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tengge1/ShadowEditor, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/shadoweditor

## Pinned environment

- Project commit: `49a6e7d506d3e859bfcfe6f175896f7c72d7a10a`
- Test commit: `49a6e7d506d3e859bfcfe6f175896f7c72d7a10a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.8 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 10.8 | 7 | 7 | [run](https://argusic.com/run/e59e9da4-5738-4826-a3aa-74e00237b4aa) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.14.3 required but not pre-installed; downloaded from go.dev`
- 2 min: `MongoDB 7.0.14 required but not pre-installed; downloaded from mongodb.com`
- 1 min: `npm dependencies not pre-installed`
- `TestGetCurrentUser fails: 'Administrator role is not found' in MongoDB`
- `TestPost fails: passport.baidu.com returns 404 (external dependency)`
- `TestTraction fails: transactions require replica set, not standalone`
- `TestTimeFormat fails: UTC timezone prints Z instead of +08:00`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
