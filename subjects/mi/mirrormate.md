# mirrormate

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/orangekame3/mirrormate, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mirrormate

## Pinned environment

- Project commit: `9cb7eae7c3012968e3f4867109ab432697a21a9d`
- Test commit: `9cb7eae7c3012968e3f4867109ab432697a21a9d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.4 to 10.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9.3 | 10.4 | 5 | 5 | [run](https://argusic.com/run/c5a6b832-050b-425a-be84-3a0ef913102a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `bun official installer failed: unzip is required`
- 1 min: `vitest crashed with ERR_REQUIRE_ESM because container had Node 18`
- 2 min: `better-sqlite3 native module segfaulted (built against system libnode.so.109)`
- 1 min: `chat API returned 500: OPENAI_API_KEY not configured / config not found`
- 1 min: `default providers.yaml points at http://studio:11434 which does not exist in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
