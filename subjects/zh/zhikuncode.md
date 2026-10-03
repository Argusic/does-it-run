# zhikuncode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zhikunqingtao/zhikuncode, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/zhikuncode

## Pinned environment

- Project commit: `0d39e2ddb966de6a83a976e3dbd68a03725ea82b`
- Test commit: `0d39e2ddb966de6a83a976e3dbd68a03725ea82b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.6 to 18 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 9.6 | 5 | 5 | [run](https://argusic.com/run/3448bd80-5c77-4a92-bd97-a3a0a0e39fbb) |
| 2 | pass | 100 | 21 | 18 | 4 | 4 | [run](https://argusic.com/run/c469b959-c769-4f7c-9be2-48d30619cef8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `JDK 21 not installed in container`
- 1 min: `Maven not installed in container`
- 1 min: `Frontend vitest failed with ERR_REQUIRE_ESM on html-encoding-sniffer via jsdom 29.x`
- `Python watchfiles test: Too many open files (os error 24) from inotify watcher`
- `Python test_estimate_batch timing assertion (988ms > 500ms boundary)`

Attempt 2:

- 1 min: `Missing Python dependency: jsonpath-ng`
- 3 min: `jsdom@29 requires Node >=20 (container has 18); ESM-only @exodus/bytes cannot be require()d`
- 3 min: `No JDK 21 available in container (no root)`
- `Log4j2 could not create /work/log directory (relative path ../log resolved outside repo)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
