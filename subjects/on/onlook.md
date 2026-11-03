# onlook

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/onlook-dev/onlook, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/onlook

## Pinned environment

- Project commit: `423e2e924366419e418ee049093872d535eea41a`
- Test commit: `423e2e924366419e418ee049093872d535eea41a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 6.5 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 6.5 | 3 | 3 | [run](https://argusic.com/run/ba1f7564-48b2-4e82-ad7d-ea54ccd26cce) |
| 2 | pass with mocks | 92 | 12 | 10 | 5 | 5 | [run](https://argusic.com/run/3ad422b0-a131-4bf7-a657-82f9fe9f5edf) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `unzip not installed; Bun installer requires it`
- 3 min: `Node.js 18.19.1 too old for Next.js (>=20.9.0 required)`
- 2 min: `6 required env vars missing in Next.js build validation`

Attempt 2:

- 2 min: `Bun not installed in container (install script failed: no unzip)`
- 3 min: `Node 18.19.1 too old for Next.js 16 (requires >=20.9.0), next build exited 1`
- 2 min: `next start backgrounded via sh exited immediately (SIGTERM) before serving`
- `Docker unavailable and no root, so supabase backend (bun backend:start, db:push, db:seed) cannot run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
