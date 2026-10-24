# Cotal

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Cotal-AI/Cotal, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cotal

## Pinned environment

- Project commit: `1793d6c635a81611f416ff6d1ce61a8a868505d4`
- Test commit: `1793d6c635a81611f416ff6d1ce61a8a868505d4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.4 to 10.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 10 | 10.4 | 2 | 1 | [run](https://argusic.com/run/355bed6f-0654-4386-91a9-d133905124b9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `cotal up preflight refused due to group-writable /home/runner/.local directory (mode 0775) , the nats-server binary path was not protected against other local writers`
- `CI gate-inventory smoke failed with 15 ungated exemptions past their recheckBy date 2026-10-24 , a process/maintenance issue, not a code defect`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
