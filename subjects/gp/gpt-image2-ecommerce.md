# gpt-image2-ecommerce

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/buluslan/gpt-image2-ecommerce, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/gpt-image2-ecommerce

## Pinned environment

- Project commit: `73abd50bf2b689b5a453f28ddd7b0016415deec6`
- Test commit: `73abd50bf2b689b5a453f28ddd7b0016415deec6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 7.2 | 1 | 1 | [run](https://argusic.com/run/bfcf9d47-0a8f-4709-b9dd-c40afdcb825f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `collect_api_response in scripts/imagegen.sh silently fails under set -euo pipefail when endpoint returns no cost info (line 591: [[ -n "$FINAL_COST" ]] && log_event ... returns exit 1 on empty FINAL_COST)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
