# argo

**Verdict: runs.** Argusic Score 98.2 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/taxueseek/argo, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/argo

## Pinned environment

- Project commit: `32428bc90aae9fe111dceec3d5ab2e89a2bad070`
- Test commit: `32428bc90aae9fe111dceec3d5ab2e89a2bad070`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 60.5 to 60.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 98.18 | 65 | 60.5 | 11 | 10 | [run](https://argusic.com/run/ff37f4aa-0436-41cb-acf6-ecf3c13feb58) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pip3 install pyyaml rejected: externally-managed-environment (PEP 668)`
- 1 min: `pytest missing in venv`
- 8 min: `test_cdp_network_idle/test_chrome_leak_fix failed: FileNotFoundError Chrome not found`
- 10 min: `test_fallback_extract/test_local_360_jisilu/test_local_baidu_pipeline/test_local_search_redirect_resolve/test_serp_guard failed: no BeautifulSoup (bs4)`
- 2 min: `test_time_filter TestCliEngineRetry failed: ddgs not available`
- 4 min: `test_cli_stdin_and_positional failed: FileNotFoundError 'argo' (tests invoke bare 'argo' on PATH)`
- 15 min: `test_fetch_v3_identity_branch/test_tinyfish_fallback/test_evidence_loop failed: 'blocked' due to SSRF guard on unresolvable fixture domains (offline DNS can't resolve v.com/docs.example.com)`
- 6 min: `test_platform_paths_conventions env-cache test failed: overlayfs keeps mtime_ns unchanged on equal-size back-to-back rewrite, cache returned stale value`
- 12 min: `test_funnel/test_race_fast_budget/test_lowlevel_smoke failed after installing rapidfuzz: fuzzy near-dup layer auto-enabled and collapsed template rows differing only by index`
- 5 min: `test_local_image 5 tests failed: FileNotFoundError 'swiftc' (Vision helper needs macOS)`
- 2 min: `health_check.py --all reports 0/18 local engines available (anti-bot, HTTP 302/400/422/429, redirect loop)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
