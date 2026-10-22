# vmprint

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cosmiciron/vmprint, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/vmprint

## Pinned environment

- Project commit: `a69394f06aa08bd97da11f92a718758eb5ea403d`
- Test commit: `a69394f06aa08bd97da11f92a718758eb5ea403d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.1 to 18.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 3 | 18.1 | 4 | 0 | [run](https://argusic.com/run/7be44515-abee-44db-b31e-3a7d2c79943b) |

## What was observed on a clean machine

Attempt 1:

- `npm install warned EBADENGINE for commander@14, lru-cache@11, rimraf@6 (require Node >=20; container has Node 18.19.1)`
- 30 min: `README/QUICKSTART example (story with inline content, no styles) fails loadDocument and lays out 0 pages; story text only flows via children`
- 40 min: `QUICKSTART code path broken: PdfContext has no waitForFinish(); renderLayout ignores the passed fontManager and crashes on getFontRegistrySnapshot`
- `vmprint --render-from-layout does not write the PDF (only end() is called)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
