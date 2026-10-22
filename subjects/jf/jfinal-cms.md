# jfinal_cms

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jflyfox/jfinal_cms, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/jfinal-cms

## Pinned environment

- Project commit: `6b5007534c4c3f11111901c377abe9efa9bb0a98`
- Test commit: `6b5007534c4c3f11111901c377abe9efa9bb0a98`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 10.5 to 23.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 10 | 10.5 | 7 | 7 | [run](https://argusic.com/run/940d3390-cf9f-43b3-a769-aa359e803a8d) |
| 2 | fail | 20 | n/a | 23.9 | 0 | 0 | [run](https://argusic.com/run/bb330ae6-017f-498f-b9a2-60676bced259) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `JDK 21 not installed`
- 1 min: `Maven not installed`
- 1 min: `Duplicate pom.xml deps cause build failure`
- 2 min: `libaio.so.1 missing for MySQL binary`
- 1 min: `libncurses.so.5 and libtinfo.so.5 missing for mysql client`
- 1 min: `MySQL root password not set and wrong port`
- 2 min: `Background MySQL/Tomcat killed between commands`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
