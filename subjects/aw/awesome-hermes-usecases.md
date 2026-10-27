# awesome-hermes-usecases

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aliaihub/awesome-hermes-usecases, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/awesome-hermes-usecases

## Pinned environment

- Project commit: `6461920777cb5f643e355be0b11dca03c1c36adf`
- Test commit: `6461920777cb5f643e355be0b11dca03c1c36adf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.3 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 12.3 | 4 | 4 | [run](https://argusic.com/run/6e328073-e346-43f4-9b9e-ab750739c18f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `fetch_json() lacked User-Agent header, causing 403 rate-limit errors from GitHub API`
- 3 min: `Original GITHUB_URL_RE regex did not capture .git suffix, causing repo name to include .git`
- 4 min: `URL with parentheses e.g. deepwiki.com/.../3.3-tui-(terminal-user-interface) got truncated by URL parser`
- `weather-trading-polymarket.md has zero source URLs or GitHub repo links, scores 0/100`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
