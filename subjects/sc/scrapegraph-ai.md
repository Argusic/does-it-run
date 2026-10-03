# Scrapegraph-ai

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ScrapeGraphAI/Scrapegraph-ai, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/scrapegraph-ai

## Pinned environment

- Project commit: `c75c8084fae2d4f5ba01a8c218bc1168b67e3569`
- Test commit: `c75c8084fae2d4f5ba01a8c218bc1168b67e3569`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 8.5 to 45.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 8.5 | 0 | 0 | [run](https://argusic.com/run/b63c13c7-8cf6-44a7-9961-32be88d6ccad) |
| 2 | pass with mocks | 92 | 2 | 45.9 | 13 | 13 | [run](https://argusic.com/run/b808bfad-a5f7-4364-971e-8731813d4fac) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `test_cleanup_html_success: minify_html library strips <body>/</body> tags`
- 1 min: `test_reduce_html_reduction_2: truncation at 20 chars gives 'Long text with more ' not 'Long text with more t'`
- 2 min: `test_llm_missing_tokens: logger.warning writes to stderr, test checked capsys.out`
- 1 min: `test_fetch_{json,xml,csv,txt}: relative file paths not resolved from test directory`
- 1 min: `test_fetch_csv: pandas not installed`
- 3 min: `robot_node_test: mock patched on wrong attribute (instance attr vs import path)`
- 3 min: `search_internet_node_test and search_link_node_test: require real ChatOllama server`
- 1 min: `test_chromium: MockBrowser missing close(), MockContext missing add_init_script`
- 1 min: `test_plasmate: patched scrapegraphai.docloaders.plasmate.ChromiumLoader which does not exist as attribute`
- 1 min: `test_script_creator_multi_graph: entry_point is a string, test compared it to node object`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
