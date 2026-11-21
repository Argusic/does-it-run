# newspaper4k

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AndyTheFactory/newspaper4k, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/newspaper4k

## Pinned environment

- Project commit: `b53a81fc01ff54601faaeae68d6b4a6d2f18efcb`
- Test commit: `b53a81fc01ff54601faaeae68d6b4a6d2f18efcb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 7.3 to 37.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 37.9 | 4 | 4 | [run](https://argusic.com/run/2cb46e4f-2078-4127-8dc1-04fd0b667cd1) |
| 2 | pass with mocks | 92 | 3 | 7.3 | 3 | 3 | [run](https://argusic.com/run/a1d308df-0801-4ffe-b721-0f59bc5c37c8) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `pytest collection failed: optional extras not installed (gnews, nltk, pythainlp, indic-nlp-library, jieba, tinysegmenter, protego) - import-time ImportError in tests and language tokenizers`
- 45 min: `tests/unit/test_nlp.py::test_summarize and test_known_websites (summary fields) failed: split_sentences/summarize under nltk 3.10.3 produce different summary than fixtures`
- 15 min: `tests/integration/test_languages.py::test_language_articles failed on chinese_article: fixture is a gb2312 page whose expected txt uses curly quotes; live page has no matching charset header`
- 20 min: `tests/integration network tests failed: test_follow_read_more_button (web.archive.org 429 rate-limit block), test_detect_binary (media.chinadaily.com.cn DNS NXDOMAIN in this container), test_multithread_sources (euronews site returns malfor`

Attempt 2:

- 1 min: `pip install failed due to PEP 668 system package protection`
- `pytest not found after pip install - installed dev deps separately`
- 4 min: `2 unit tests failed due to NLTK 3.10+ sentence tokenizer changes (punkt_tab)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
