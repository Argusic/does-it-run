# moemail

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/beilunyang/moemail, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/moemail

## Pinned environment

- Project commit: `5722ceb2fca1d4f7a957ba09e93492d1c7b5d02f`
- Test commit: `5722ceb2fca1d4f7a957ba09e93492d1c7b5d02f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 11.6 to 25.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 5 | 11.6 | 3 | 0 | [run](https://argusic.com/run/0eb0c583-75c4-4752-8bbc-e725783c8c8a) |
| 2 | pass with mocks | 92 | 25 | 25.7 | 3 | 3 | [run](https://argusic.com/run/ce7b169b-5294-4ab0-8a4a-812de4b7c802) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Pnpm build scripts ignored for bun, esbuild, sharp, workerd (non-fatal; packages still installed)`
- 3 min: `Next.js build OOM killed - container has insufficient memory for production build`
- `Cloudflare API token not available - cannot create remote D1 database or test email sending`

Attempt 2:

- 10 min: `pnpm v12 block on build scripts (ERR_PNPM_IGNORED_BUILDS) - could not approve non-interactively`
- 5 min: `Next.js production build OOM-killed (exit 137) during static page generation`
- 2 min: `CLI built with bun but bundler (bun) not in PATH - bun binary named bun.exe`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
