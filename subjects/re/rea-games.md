# rea-games

**Verdict: runs.** Argusic Score 86.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/erkamyaman/rea-games, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/rea-games

## Pinned environment

- Project commit: `4480ef0474b65c0fadebbab89245ea1eb31682c5`
- Test commit: `4480ef0474b65c0fadebbab89245ea1eb31682c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.4 to 1.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 0.6 | 1.4 | 3 | 1 | [run](https://argusic.com/run/d0a9569a-f0e9-4c7b-b0df-d46f184a1f50) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18 on system; project requires >=22`
- `Godot ports fail: no Godot binary`
- `Bevy/Rust ports fail: no cargo/rustc`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
