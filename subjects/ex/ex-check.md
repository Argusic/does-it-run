# ex_check

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/karolsluszniak/ex_check, licensed MIT, written in Elixir.

Evidence and recordings: https://argusic.com/subject/ex-check

## Pinned environment

- Project commit: `50b761188efa81593dca3d83729f835d828ac2da`
- Test commit: `50b761188efa81593dca3d83729f835d828ac2da`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.2 to 15.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 4 | 15.2 | 1 | 0 | [run](https://argusic.com/run/ee252658-eb22-440b-891c-df3c8ce9cbbb) |

## What was observed on a clean machine

Attempt 1:

- `mix check --format agent: hex_audit failed due to CVE advisories in transitive deps mint (3 CVEs) and decimal (1 CVE)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
