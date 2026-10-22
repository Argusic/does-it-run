# paozhu

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hggq/paozhu, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/paozhu

## Pinned environment

- Project commit: `a6094e298dab2f5191e47b7dd6fd89f156590406`
- Test commit: `a6094e298dab2f5191e47b7dd6fd89f156590406`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.6 to 17.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 55 | 17.6 | 5 | 5 | [run](https://argusic.com/run/7e592936-2198-47c9-9b1c-9ed2d443c456) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing Asio standalone headers (asio.zip not extracted)`
- 5 min: `Brotli headers not found (brotli/encode.h)`
- 3 min: `Brotli static link: undefined references to _kBrotliPrefixCodeRanges etc.`
- 2 min: `cmake file(MAKE_DIRECTORY /usr/local/etc/paozhu) fails with Permission denied`
- 10 min: `Missing zlib/brotli/sqlite3 -dev headers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
