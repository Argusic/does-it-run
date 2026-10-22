# metis

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Wholiver/metis, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/metis

## Pinned environment

- Project commit: `fb56c019b2a04a98a0b903195a246fc9ef959241`
- Test commit: `fb56c019b2a04a98a0b903195a246fc9ef959241`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 34.2 to 34.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.3 | 34.2 | 3 | 3 | [run](https://argusic.com/run/043b9adb-d7ce-4e6d-bbe7-a671f2e74de9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Electron chrome-sandbox not SUID root (non-root container)`
- `test/desktop-chat-scroll.test.ts: Electron requestAnimationFrame hangs with full Tailwind CSS in headless GPU-less env`
- `test/terminalbench-adapter.test.ts: adapters/harbor_tb/agent.py missing (excluded from npm package)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
