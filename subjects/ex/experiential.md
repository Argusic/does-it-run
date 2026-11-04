# experiential

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/experientiallabs/experiential, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/experiential

## Pinned environment

- Project commit: `1253c82fe479a195e6b63d2ef215d28f6cc39c9c`
- Test commit: `1253c82fe479a195e6b63d2ef215d28f6cc39c9c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 70.3 to 74 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 70.3 | 2 | 2 | [run](https://argusic.com/run/50e95f7f-6493-4935-bcff-be726864beba) |
| 2 | pass | 100 | 45 | 74 | 7 | 7 | [run](https://argusic.com/run/9106a79c-4f81-4d29-a654-148bfa5445fa) |

## What was observed on a clean machine

Attempt 1:

- `ty check: 38 unresolvable import errors for mitmproxy, mitmproxy_rs, and brotli in capture modules (Python 3.12, needs 3.13)`

Attempt 2:

- 2 min: `uv not installed in container`
- 6 min: `rustc/cargo not installed; native gateway crate requires them`
- 15 min: `uv sync on system Python 3.12 left venv incomplete; repo gates need 3.13`
- 10 min: `TERM unset made ~77 rich picker PTY tests fail (non-interactive fallback)`
- 5 min: `test_prepared_snapshot_rejects_path_and_content_races[rewrite] fails on overlayfs ctime semantics in this container`
- 3 min: `macOS-only capture lock test fails on Linux because pwd exists and ~/Library 0755 trips fail-closed ancestor check`
- 2 min: `my CLI guesses for alias streaming flag and key-id pattern were wrong`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
