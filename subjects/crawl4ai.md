# crawl4ai

**Verdict: runs.** Argusic Score 91.4 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/unclecode/crawl4ai, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/crawl4ai

## Pinned environment

- Project commit: `e5d2e786d1a101225f3f6a3e6fd344d76eeb13af`
- Test commit: `e5d2e786d1a101225f3f6a3e6fd344d76eeb13af`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.2 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 91.43 | 25 | 14.2 | 14 | 8 | [run](https://argusic.com/run/2677f1e7-2578-439c-a405-42bbf0afa12c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PEP 668 externally-managed-environment blocks system pip`
- 1 min: `playwright install --with-deps requires root`
- 0.5 min: `pypdf missing for PDF content scraping`
- 2 min: `normalize_url empty href returned None instead of base URL`
- 0.5 min: `normalize_url dropped #fragment by default`
- 1 min: `normalize_url no ValueError on invalid base URL (ftp://, http:///path/)`
- 3 min: `AsyncWebCrawler missing aclear_cache, aflush_cache, aget_cache_size`
- 1 min: `BaseDispatcher.select_config returns None on no match, tests expect first config`
- `Test files with dots in name (test_0.4.2_*) can't be collected by pytest`
- `test_http_crawler_strategy.py imports tkinter (not installed)`
- `test_scraping_strategy.py imports nest_asyncio (not installed)`
- `test_content_scraper_strategy.py imports tabulate (not installed)`
- `test_crawlers.py imports get_crawler which doesn't exist`
- `test_schema_builder.py imports JsonXPathExtractionStrategy from wrong module`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
