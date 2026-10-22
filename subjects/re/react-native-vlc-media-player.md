# react-native-vlc-media-player

**Verdict: could not verify.** Argusic Score 40 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/razorRun/react-native-vlc-media-player, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/react-native-vlc-media-player

## Pinned environment

- Project commit: `8f7affb1755dbb044ad7daa43a5cdef60ebd41bf`
- Test commit: `8f7affb1755dbb044ad7daa43a5cdef60ebd41bf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.7 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 1.5 | 5.7 | 1 | 1 | [run](https://argusic.com/run/8847e52d-5111-4bca-9091-211a6603d759) |
| 2 | fail | 30 | 1.2 | 6 | 1 | 0 | [run](https://argusic.com/run/a348ecf0-b4e9-4cc5-8c24-d587bb01cb98) |

## What was observed on a clean machine

Attempt 1:

- `npm test exits 1 by design: 'Error: no test specified'`

Attempt 2:

- 0.2 min: `Package has no test suite - 'npm test' echoes 'Error: no test specified' and exits 1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
