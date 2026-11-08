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
- Valid runs: 2; wall time 2.2 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15.2 | 2.2 | 1 | 1 | [run](https://argusic.com/run/b9f95b51-1283-474b-b40f-7602c5b00066) |
| 2 | pass | 100 | 10 | 3.4 | 3 | 3 | [run](https://argusic.com/run/6f68b792-c243-4956-bf23-5c1d4fc93812) |

## What was observed on a clean machine

Attempt 1:

- 14.5 min: `npm run check failed because AGENT_NATIVE_FRAMEWORK_PATH was not set and ../agent-native/framework did not exist`

Attempt 2:

- 2 min: `Missing agent-native framework dependency (clone of BuilderIO/agent-native repo at ../agent-native)`
- 1 min: `visual-edit/SKILL.md out of sync with upstream agent-native`
- 1 min: `npx @agent-native/skills@latest add fails on Node 18 (requires >=22.22.0)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
