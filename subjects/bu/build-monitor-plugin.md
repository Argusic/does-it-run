# build-monitor-plugin

**Verdict: runs with mocks.** Argusic Score 88 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jenkinsci/build-monitor-plugin, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/build-monitor-plugin

## Pinned environment

- Project commit: `9b89ddc60c591976cd6ff0e78eaa734e278b86a9`
- Test commit: `9b89ddc60c591976cd6ff0e78eaa734e278b86a9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 37.6 to 37.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 88 | 92 | 37.6 | 5 | 4 | [run](https://argusic.com/run/e037698c-2a6e-484a-8fdd-94225a7e4995) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Java, Maven, or Node>=22 in container (Node was 18; project requires Node>=22)`
- 2 min: `Maven tarball download failed: HTML page instead of gzip`
- 30 min: `Standalone Jenkins could not load the HPI: missing dependency jackson2-api plus 'expected build-monitor-plugin.jpi' naming`
- 15 min: `curl form submissions to Jenkins view-creation URLs 404'd on this Jenkins baseline`
- 25 min: `Playwright host check: 'Host system is missing dependencies to run browsers' (libwoff1, libgstreamer*, libharfbuzz-icu0, etc.), no root to apt-install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
