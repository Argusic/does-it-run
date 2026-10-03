# uilayouts

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ui-layouts/uilayouts, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/uilayouts

## Pinned environment

- Project commit: `88d827d7ec342917ca06f6894e5add65fabbe5d8`
- Test commit: `88d827d7ec342917ca06f6894e5add65fabbe5d8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 4; wall time 15.6 to 31.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.33 | 18.6 | 3 | 3 | [run](https://argusic.com/run/a7b0005b-acf1-4392-9d17-bd8a4fc4f1a2) |
| 1 | fail | 80 | 1.2 | 15.6 | 3 | 3 | [run](https://argusic.com/run/b59c6cfd-3baa-4e63-b2de-e86a2cf87df1) |
| 2 | pass | 100 | 25 | 23.8 | 4 | 4 | [run](https://argusic.com/run/b1ea74bc-be86-4bfe-ae82-312799a8b609) |
| 3 | pass | 100 | 14 | 31.7 | 4 | 4 | [run](https://argusic.com/run/70596ab8-c4c5-4621-80f2-787f72d5b2f7) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `packages/ui and packages/shadcn tsconfig paths reference files outside rootDir causing tsc build failure`
- 5 min: `@tailwindcss/oxide native binding not installed (optional dependency missing)`
- 4 min: `next build OOM during static page generation (exit 137)`

Attempt 1:

- 2 min: `@repo/ui package build failed: files banner.tsx and tree.tsx imported cn from '@/lib/utils' which resolves outside the package rootDir via tsconfig paths`
- 1 min: `@tailwindcss/oxide native binding not installed - optional dependency @tailwindcss/oxide-linux-x64-gnu was missing`
- `Next.js production build gets killed during 'Collecting page data' phase, likely OOM (only ~450MB free, no swap)`

Attempt 2:

- 2 min: `pnpm not available on system; host node v18.19.1`
- 10 min: `@tailwindcss/oxide-linux-x64-gnu native binding missing - pnpm did not install the optional dependency for linux-x64-gnu`
- 5 min: `Turbo build fails on packages/ui - @/lib/utils path alias points outside the package rootDir to apps/ui-layout/lib/utils, causing TS6059`
- 8 min: `next build killed by OOM during 'Collecting page data' phase (exit 137) despite available memory`

Attempt 3:

- 3 min: `@repo/ui build failed: tsconfig paths @/lib/*, @/components/*, @/hooks/* pointed outside rootDir`
- 5 min: `@repo/shadcn build failed: missing radix-ui package, @/hooks/use-mobile not found, @/components/website/ui/label not found`
- 3 min: `Next.js build failed: @tailwindcss/oxide native binding not installed for linux-x64-gnu`
- 2 min: `Next.js build OOM during 'Collecting page data' phase (exit code 137)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
