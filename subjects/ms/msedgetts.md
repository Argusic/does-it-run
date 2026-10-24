# MsEdgeTTS

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Migushthe2nd/MsEdgeTTS, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/msedgetts

## Pinned environment

- Project commit: `40a59155a6977192fb71a473e6bd97dad97798ec`
- Test commit: `40a59155a6977192fb71a473e6bd97dad97798ec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 26 to 26 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.1 | 26 | 4 | 4 | [run](https://argusic.com/run/494eb656-6745-4516-aaf9-5cfef8a5dcd3) |

## What was observed on a clean machine

Attempt 1:

- 0.4 min: `pnpm not pre-installed; installed via npm to ~/.local/bin`
- 5 min: `Jest sandbox strips globalThis.crypto in Node 18 , ReferenceError on crypto.subtle.digest and crypto.getRandomValues`
- 8 min: `Tests connecting to real Microsoft Edge TTS API get HTTP 403 , no network access to the endpoint`
- 3 min: `Metadata stream not closed on turn.end causing toFile to hang for metadata test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
