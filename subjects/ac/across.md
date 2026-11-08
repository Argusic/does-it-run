# across

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/teddysun/across, licensed Apache-2.0, written in Shell.

Evidence and recordings: https://argusic.com/subject/across

## Pinned environment

- Project commit: `fdb40962837b2e24bc94b87c2b1786ad2308489a`
- Test commit: `fdb40962837b2e24bc94b87c2b1786ad2308489a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.7 to 18.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0 | 18.4 | 1 | 1 | [run](https://argusic.com/run/958a29d8-b4cd-486c-9440-3ea46fa473bb) |
| 2 | pass | 100 | 0.2 | 6.7 | 1 | 1 | [run](https://argusic.com/run/b5643c94-d609-4754-aca2-ea6420b602ca) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `wget not found in container, bench.sh speedtest download failed`

Attempt 2:

- 0.3 min: `wget not installed; bench.sh uses hardcoded wget for speedtest download (has curl-based fallback for geo-IP only)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
