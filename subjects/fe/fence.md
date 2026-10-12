# fence

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fencesandbox/fence, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/fence

## Pinned environment

- Project commit: `737751a82b49f287b41f8a3e62ec62919d7b9224`
- Test commit: `737751a82b49f287b41f8a3e62ec62919d7b9224`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 9.8 to 18.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 10 | 18.9 | 4 | 4 | [run](https://argusic.com/run/3f58ee47-6697-4134-a2f8-b5e9002df9aa) |
| 2 | fail | 20 | n/a | 9.8 | 0 | 0 | [run](https://argusic.com/run/db81fa70-da55-493a-a68e-a25022d9c1df) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go not pre-installed; had to download Go 1.26.0 and set PATH`
- 2 min: `bubblewrap (bwrap) not found; required for Linux sandboxing`
- 2 min: `socat not found; required for network bridging`
- 5 min: `bwrap: kernel does not allow non-privileged user namespaces , all sandbox integration tests fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
