# SeleniumBase

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/seleniumbase/SeleniumBase, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/seleniumbase

## Pinned environment

- Project commit: `5de2d4679d5171bdffcbb5b1f3ab5fbca2c8ddd3`
- Test commit: `5de2d4679d5171bdffcbb5b1f3ab5fbca2c8ddd3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 5 to 26.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 26.2 | 5 | 5 | [run](https://argusic.com/run/5cf3a243-37b6-4122-b43f-e0a89ecd0bbf) |
| 2 | pass | 100 | 2.5 | 20.6 | 4 | 4 | [run](https://argusic.com/run/9d1fb5da-a6d3-4101-9f20-a63d087d60b2) |
| 3 | pass | 100 | 2 | 5 | 0 | 0 | [run](https://argusic.com/run/40824656-fcdc-4318-9ea2-a23099a053a0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No system browser installed on container`
- `test_override_driver fails - raw webdriver.Chrome() without --no-sandbox in sandboxed env`
- `test_override_sb_fixture fails - same raw Chrome options issue`
- `test_geolocation fails - external site changed content`
- `test_detect_404s fails by design (checks known-broken page)`

Attempt 2:

- 1 min: `Externally-managed Python environment prevents system-wide pip install`
- 0.8 min: `Default chromedriver 114 does not match Playwright Chromium 153`
- 0.2 min: `seleniumbase get chromedriver tries to copy to /usr/local/bin (Permission denied)`
- 0.1 min: `pytest --timeout flag rejected by SeleniumBase plugin`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
