# doca

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/smartdoca/doca, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/doca

## Pinned environment

- Project commit: `091efcd458482348205ed5856b46355725fa6d27`
- Test commit: `091efcd458482348205ed5856b46355725fa6d27`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 31.2 to 31.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 31 | 31.2 | 7 | 7 | [run](https://argusic.com/run/8573f35e-c0a2-4226-905f-68243572ef96) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Container provides Node v18.19.1 and no pnpm, but the repo requires Node >=22 and pnpm 11.25.0 (packageManager field); install could not start`
- 4 min: `Ran 'pnpm dev', confirmed 200 on web and API, then both ports refused connections; dev server had been killed when the launching shell exited`
- 2 min: `POST /api/v1/files/items with Content-Type text/markdown returned HTTP 415 'service unavailable'`
- 10 min: `'pnpm test' failed 97 tests in 11 files with 'trusted_engine_required'; root cause was the container umask 0002 making temp dirs group-writable (0775), which the segmentation security check rejects`
- 4 min: `'pnpm typecheck' (tsc --noEmit) aborted with 'JavaScript heap out of memory' at Node's default heap on this large monorepo`
- 8 min: `tests/document-pdf.test.ts fails 2 tests: the renderer hardcodes chromiumSandbox:true and the downloaded Chromium headless shell cannot start ('No usable sandbox!', unprivileged user namespaces disabled by AppArmor on this Ubuntu 24.04 cont`
- 3 min: `tests/ai-document-parsing.test.ts fails 3 tests with 'spawn soffice ENOENT': DOCX/XLSX/PPTX rendering requires LibreOffice`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
