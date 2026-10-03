# WechatSogou

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chyroc/WechatSogou, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/wechatsogou

## Pinned environment

- Project commit: `6a7e08caa82dd7cf47331d7c303f578a4b325360`
- Test commit: `6a7e08caa82dd7cf47331d7c303f578a4b325360`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 5.9 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 4 | 5.9 | 6 | 6 | [run](https://argusic.com/run/678b31c7-2190-47d5-9596-cf4388c99fc6) |
| 2 | fail | 80 | 12 | 12.6 | 5 | 5 | [run](https://argusic.com/run/0673a8ba-36ee-44dc-b630-e3d13f56205c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `externally-managed-environment (PEP 668 blocked system pip)`
- 1 min: `setuptools not installed in venv (BackendUnavailable)`
- 1 min: `werkzeug.contrib.cache removed in Werkzeug 3.x`
- 2 min: `nose requires imp module removed in Python 3.12`
- 1 min: `test_const.py tested non-existent attributes (duanzi, dianzan)`
- `test_structuring.py used nose-specific assert_equal.__self__.maxDiff`

Attempt 2:

- 2 min: `lxml==4.6.2 fails to build from source (no libxml2/libxslt dev headers)`
- 1 min: `Werkzeug.contrib.cache module removed in Werkzeug>=1.0`
- 3 min: `nose test runner incompatible with Python 3.12 ('imp' module removed)`
- 1 min: `Missing hot_index constants 'duanzi' and 'dianzan' in _WechatSogouHotIndexConst`
- 1 min: `gen_hot_url index_urls dict missing entries for 'duanzi' and 'dianzan'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
