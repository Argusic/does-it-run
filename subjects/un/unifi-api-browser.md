# UniFi-API-browser

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Art-of-WiFi/UniFi-API-browser, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/unifi-api-browser

## Pinned environment

- Project commit: `972f6fadc82fe3dbf40453e7b62fb66211966c72`
- Test commit: `972f6fadc82fe3dbf40453e7b62fb66211966c72`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 7.5 | 3 | 3 | [run](https://argusic.com/run/7a6929d1-2300-46c7-9a80-57a238d6fdfa) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP CLI not installed - needed to run the application`
- 2 min: `PHP curl extension not loaded - required by the UniFi-API-client`
- 1 min: `PHP session save_path (/var/lib/php/sessions) not writable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
