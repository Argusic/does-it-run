# franz

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/meetfranz/franz, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/franz

## Pinned environment

- Project commit: `94b1ef298aa72a41eac448f4e5e21a74d857f2fa`
- Test commit: `94b1ef298aa72a41eac448f4e5e21a74d857f2fa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 3.9 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 3.9 | 1 | 1 | [run](https://argusic.com/run/34aeffb5-9276-46c3-b617-a3be1c79042c) |
| 2 | pass | 100 | 1.5 | 7.5 | 3 | 3 | [run](https://argusic.com/run/cff46fcc-b183-4cbd-a223-76b71cfc9e68) |
| 3 | pass | 100 | 8 | 9.6 | 3 | 3 | [run](https://argusic.com/run/98db214f-b54b-43e4-856a-b34fe055ae07) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `npm run dev failed because gulp-server-livereload uses fs.watch recursive which is unavailable on Node 18 on this Linux platform`

Attempt 2:

- 2 min: `npx lerna bootstrap failed - lerna@10 incompatible with Node 18`
- `gulp build minify task never completed (terser async issue)`
- `gulp dev webserver failed - fs.watch recursive not available on platform`

Attempt 3:

- 2 min: `Bundled npm@6.14.8 in package.json forces npm 6 which is incompatible with lockfile v2, causing bootstrap failure with ENOENT on packages/forms/node_modules/@mdi/js`
- 1 min: `lerna@latest (10.x) requires Node >=22 but container has Node 18`
- 2 min: `TypeScript build fails for @meetfranz/ui and @meetfranz/forms because they cannot find @meetfranz/theme in their own node_modules (lerna hoists to root only)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
