# xxl-crawler

**Verdict: runs.** Argusic Score 91.4 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xuxueli/xxl-crawler, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/xxl-crawler

## Pinned environment

- Project commit: `2088dd10212f42a9741a6d7b59526400d8317237`
- Test commit: `2088dd10212f42a9741a6d7b59526400d8317237`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.6 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 91.43 | 12 | 12.6 | 7 | 4 | [run](https://argusic.com/run/6c0c5d2e-3fbf-4d55-ab9d-e8a9b872c829) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Java 17 or Maven in container`
- 1 min: `CrawlerUtilTest failed: AccessDenied at /Users/admin/Downloads/tmp (macOS path)`
- 1 min: `JsoupUtilTest.findImagesTest failed: NPE when JsoupUtil.load() returns null (rate limit on baidu.com)`
- 2 min: `Surefire did not discover tests named XxlCrawlerTest01 (numbers in suffix)`
- `XxlCrawlerTest05 (Selenium+ChromeDriver) needs chromedriver binary not in container`
- `XxlCrawlerTest06 (proxy) needs real proxy IPs not available`
- `XxlCrawlerTest07 (Redis/RunUrlPool) needs Redis running and throws XxlCrawlerException as design`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
