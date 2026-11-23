# letterpad

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/letterpad/letterpad, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/letterpad

## Pinned environment

- Project commit: `91d3e2516987ea00b1f068bda20dcd8fd14eb90d`
- Test commit: `91d3e2516987ea00b1f068bda20dcd8fd14eb90d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 23.5 to 39.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 50 | 39.1 | 4 | 4 | [run](https://argusic.com/run/b7b8e00e-b135-4364-a1d4-969186b1705c) |
| 2 | pass | 100 | 28 | 23.5 | 8 | 8 | [run](https://argusic.com/run/65c34434-d6e7-40f4-bf02-14f9e54f0558) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Bun is not installed in the container`
- 15 min: `Bun lifecycle scripts fail with '/bin/sh: Bad substitution' because dash cannot run the repo's bash [[ ]] scripts`
- 25 min: `Production build ('bun run build') is SIGKILLed by the 8GB cgroup OOM limit during Next static generation in both apps`
- 5 min: `Database seed failed with Prisma errors for missing required Author fields (bio, occupation, password)`

Attempt 2:

- 2 min: `bun not installed in container`
- 1 min: `DATABASE_URL not set during install causing prisma prepare failure`
- 5 min: `Seed script fails: Author model requires bio, occupation, company_name fields but createAuthorWithSettings doesn't provide defaults`
- 2 min: `letterpad-graphql package.json exports missing 'require' entry for CJS`
- 3 min: `Prisma SQLite schema missing likes/views fields on Tag model (present in MySQL schema)`
- 10 min: `Multiple TypeScript strict null/type errors in onboard/index.ts, getMedia.ts, updateMedia.ts, createPost.ts, getPosts.ts, formatHtml.ts, subscriber.ts, getTags.ts, dbTypeCheck.ts, [...nextauth].ts, helpers.ts`
- 1 min: `React.cache polyfill needed for Jest (React 18 doesn't have cache)`
- 2 min: `Admin Next.js build SIGKILL during static page generation (0/56)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
