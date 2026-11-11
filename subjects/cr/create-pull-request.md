# create-pull-request

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/peter-evans/create-pull-request, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/create-pull-request

## Pinned environment

- Project commit: `11e8dc7c9cc95aabee9cfaa85faaec8b50907340`
- Test commit: `11e8dc7c9cc95aabee9cfaa85faaec8b50907340`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.4 to 35.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 15.4 | 4 | 4 | [run](https://argusic.com/run/ec753ceb-87da-47f7-8374-b7650a5c8cb0) |
| 2 | pass | 100 | 2 | 35.9 | 3 | 3 | [run](https://argusic.com/run/e2184a1f-eafd-46cd-a5df-7533c57c3a97) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node 18 installed, but package requires >=24.4.0; also ncc fails with 'N.hash is not a function' on Node 24`
- 1 min: `Unit tests fail because lib/ (compiled tsc output) is missing`
- 2 min: `Integration test paths hardcoded to /git/local/repos/ which is not writable in this container`
- 4 min: `Integration test runner uses Docker (not available), and git daemon needed for remote operations`

Attempt 2:

- 2 min: `Node v18 does not satisfy >=24.4.0 engine requirement`
- 1 min: `Integration test hardcodes /git/ paths not present in container`
- 3 min: `git daemon process killed between exec calls / port 9418 in TIME_WAIT`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
