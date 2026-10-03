# zvec-grep

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zvec-ai/zvec-grep, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/zvec-grep

## Pinned environment

- Project commit: `4c5b1a00402fa843c21ab81c03771a4f037b26c7`
- Test commit: `4c5b1a00402fa843c21ab81c03771a4f037b26c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 53.7 to 53.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 53.7 | 2 | 2 | [run](https://argusic.com/run/05ab1ef5-aef7-42fd-b516-ae8324056376) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18.19.1 installed but project requires >=22`
- `2 shutdown origin tests fail for IPv6 ::1 loopback`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
