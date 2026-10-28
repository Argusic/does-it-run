# pi-agent-browser-native

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fitchmultz/pi-agent-browser-native, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pi-agent-browser-native

## Pinned environment

- Project commit: `6d4f6fefa14cf00fd0bb72cc50cace295aa55871`
- Test commit: `6d4f6fefa14cf00fd0bb72cc50cace295aa55871`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 84.2 to 84.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3.5 | 84.2 | 1 | 1 | [run](https://argusic.com/run/bc12e461-044c-4701-acd4-2b7b7d1ae4cc) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `Container umask 0002 creates group-writable directories (0o775) rejected by isTrustedPosixDirectory in managed-session-storage.ts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
