# geziyor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/geziyor/geziyor, licensed MPL-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/geziyor

## Pinned environment

- Project commit: `229b8ca83ac1ff9bd17ce533622a5d915ce36f56`
- Test commit: `229b8ca83ac1ff9bd17ce533622a5d915ce36f56`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.4 to 16.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 16.4 | 6 | 6 | [run](https://argusic.com/run/900134d6-8fd6-47d4-91f6-48adc3ae32ab) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `No Go compiler in container`
- 2 min: `//go:build syntax errors in pinned deps incompatible with Go 1.16`
- 1 min: `TestPostFormUrlEncoded panics: nil map assignment`
- 1 min: `TestRetry: no error returned after retries exhausted on 500 status`
- 1 min: `TestJSONExporter_Export: trailing comma produces invalid JSON`
- `Disk space cleanup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
