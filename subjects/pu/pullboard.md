# pullboard

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pullboard-dev/pullboard, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/pullboard

## Pinned environment

- Project commit: `594e50d5cb4fad955c0e4e53fdd1f7dbda62bd84`
- Test commit: `594e50d5cb4fad955c0e4e53fdd1f7dbda62bd84`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 59.2 to 59.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 59.2 | 5 | 5 | [run](https://argusic.com/run/b1fed840-5870-4e64-9dfc-77f27d832012) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node v18.19.1 too old (requires >=22.13)`
- 3 min: `ssh-keygen not found , 21 SSH signer/signoff tests fail`
- 2 min: `No release tags in shallow clone , 11 tests fail on 'fatal: not a valid object name: v0.8.x'`
- 3 min: `Chrome not found , 23 N26 view tests skip, more than 80 view/rendering tests fail`
- `1 test 'parent death drains a detached worker descendant before releasing its lease' always fails`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
