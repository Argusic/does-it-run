# itshover

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/itshover/itshover, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/itshover

## Pinned environment

- Project commit: `65862bd1d31cbb438ee379c328bd13ddc6c319b3`
- Test commit: `65862bd1d31cbb438ee379c328bd13ddc6c319b3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 6.1 to 27.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 13.4 | 4 | 4 | [run](https://argusic.com/run/3b78c795-8047-407d-b787-648563e6be81) |
| 1 | pass | 100 | 6 | 6.1 | 2 | 2 | [run](https://argusic.com/run/7729dec0-f1fc-4cb6-ae6c-6c2c486e4382) |
| 2 | pass | 100 | 0.3 | 8.7 | 2 | 2 | [run](https://argusic.com/run/b700ffdd-4948-4ee1-9dab-b38a0a140fb4) |
| 3 | pass | 100 | 3 | 27.4 | 3 | 3 | [run](https://argusic.com/run/bdc8470e-5cc7-4521-8a42-5ba89d75c3ff) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js 18 (system) too old for Next.js 16; npm install completed but next CLI failed with engine error`
- 2 min: `npm install had ENOTEMPTY cleanup failure on first attempt leaving corrupt node_modules/next`
- 1 min: `Stale node_modules_bak directory caused TypeScript build error referencing @babel/core from old modules`
- `MONGODB_URI environment variable not set; mongoose.connect() fails on sponsor page`

Attempt 1:

- 2 min: `Node.js 18.19.1 is too old for Next.js 16.1.0 (requires >=20.9.0). npm install succeeded but next build failed with 'Node.js version >=20.9.0 required'.`
- `MONGODB_URI environment variable not set. lib/db.ts uses process.env.MONGODB_URI! which crashes mongoose.connect. Sponsor page (get-sponsors action) catches the error gracefully and returns empty array.`

Attempt 2:

- 5 min: `Node.js 18.19.1 is too old for Next.js 16.1.0 (requires >=20.9.0)`
- 2 min: `Missing environment variables: MONGODB_URI, GITHUB_ACCESS_TOKEN, NEXT_PUBLIC_UMAMI_SRC, NEXT_PUBLIC_UMAMI_ID`

Attempt 3:

- 5 min: `Node.js 18.19.1 does not satisfy Next.js 16's requirement of >=20.9.0. npm install succeeded with engine warnings but npm run build failed immediately.`
- 3 min: `ESLint config uses flat config format specific to Next.js 16 (import from 'eslint/config' and 'eslint-config-next/core-web-vitals' as flat config arrays) which doesn't exist in Next.js 15.`
- 8 min: `Build hung at 'Generating static pages (0/276)' due to MongoDB connection from getSponsors() failing to connect/hang, and server actions during static generation.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
