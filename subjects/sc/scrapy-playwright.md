# scrapy-playwright

**Verdict: runs.** Argusic Score 93.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/scrapy-plugins/scrapy-playwright, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/scrapy-playwright

## Pinned environment

- Project commit: `d99f38d3483118881add4e2bcbc595d45091f196`
- Test commit: `d99f38d3483118881add4e2bcbc595d45091f196`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 12.4 to 61 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5.5 | 61 | 5 | 5 | [run](https://argusic.com/run/e0688ff3-87ed-402c-9a8b-33c67dc54d0e) |
| 2 | pass | 95 | 2.5 | 12.4 | 4 | 3 | [run](https://argusic.com/run/28c5e9ec-65a5-4fbe-b3ce-057e3c249dc9) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing 'file' command for MIME type detection in test_page_methods.py`
- 15 min: `Firefox test classes (TestProcessHeadersFirefox, TestCaseMultipleContextsFirefox) hang indefinitely in pytest-twisted`
- 5 min: `Browser crash/reconnect tests (test_browser_crashed_restart, test_browser_crashed_do_not_restart) hang in pytest`
- 5 min: `Remote browser tests (test_connect, test_connect_devtools, test_connect_download) hang waiting for a browser server process`
- `WebKit unavailable on Linux (system dependencies missing, no root to install)`

Attempt 2:

- 1 min: `test_page_methods.py: get_mimetype() failed because 'file' command not available`
- 1 min: `test_utils.py: w3lib now maps gb2312 to gbk instead of gb18030`
- 2 min: `test_extensions.py: Playwright 1.65 changed PlaywrightContextManager internal API from _connection to _client`
- `test_browser.py tests hang: need external browser server processes (chromium with --remote-debugging-port, node browser server)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
