# OpenScribe

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sammargolis/OpenScribe, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openscribe

## Pinned environment

- Project commit: `dddf1c30fcf8313e4452915ddd9189baa5a3762b`
- Test commit: `dddf1c30fcf8313e4452915ddd9189baa5a3762b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.4 to 16.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 16.4 | 4 | 4 | [run](https://argusic.com/run/694e9e21-0df5-4dc6-bf01-3503663162a0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18.19.1 too old for Next.js 16 (needs >=20.9.0)`
- 3 min: `crypto.randomUUID() not available as bare global in Node --test workers`
- 2 min: `globalThis.crypto unavailable in Node 18 test workers, causing Web Crypto API errors in secure-storage.ts`
- 1 min: `@tailwindcss/oxide native binary missing (pnpm install ran under Node 18)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
