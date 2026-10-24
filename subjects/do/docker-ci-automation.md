# docker-ci-automation

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BretFisher/docker-ci-automation, licensed Unlicense, written in Shell.

Evidence and recordings: https://argusic.com/subject/docker-ci-automation

## Pinned environment

- Project commit: `0608ac3f115b2ed4905bf1ae9a9fb168aad6c798`
- Test commit: `0608ac3f115b2ed4905bf1ae9a9fb168aad6c798`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 2.4 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 1 | 13.6 | 2 | 2 | [run](https://argusic.com/run/7b8efcdc-9856-4e9a-94d4-6a823ba7d0ac) |
| 2 | fail | 50 | 0 | 2.4 | 0 | 0 | [run](https://argusic.com/run/311b017e-d8f1-4086-a70b-30faba70fc98) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Docker daemon could not start rootless mode: newuidmap write to uid_map failed (Operation not permitted)`
- 2 min: `act needs Docker daemon to execute workflows; cannot dry-run GitHub Actions without Docker`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
