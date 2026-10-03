# skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BuilderIO/skills, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/b9f95b51-1283-474b-b40f-7602c5b00066

## Pinned environment

- Project commit: `eb07be67e6d924b958445f706f5ac386243df6b4`
- Test commit: `eb07be67e6d924b958445f706f5ac386243df6b4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.2 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15.2 | 2.2 | 1 | 1 | [run](https://argusic.com/run/b9f95b51-1283-474b-b40f-7602c5b00066) |

## What was observed on a clean machine

Attempt 1:

- 14.5 min: `npm run check failed because AGENT_NATIVE_FRAMEWORK_PATH was not set and ../agent-native/framework did not exist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
