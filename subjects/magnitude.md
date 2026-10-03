# magnitude

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/magnitudedev/magnitude, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/magnitude

## Pinned environment

- Project commit: `b3e5a06bda3ee5b112c428718bd6983a7d772671`
- Test commit: `b3e5a06bda3ee5b112c428718bd6983a7d772671`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.4 to 26.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 25 | 26.4 | 3 | 2 | [run](https://argusic.com/run/ada227d7-74d1-475a-b317-7124e57a4642) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `git VCS tests fail: "invalid tree entry mode: '100664'" , container umask 0002 creates files with modes git rejects`
- 3 min: `utils patch tests fail: cannot find module '../../../../protocol/src/schemas/display' , protocol package renamed to acn-protocol`
- `daemon-management: 28 tests fail , missing native binaries dist/native/linux-x64/desktop-host.node and magnitude-command`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
