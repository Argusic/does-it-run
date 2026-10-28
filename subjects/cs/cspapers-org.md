# cspapers.org

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/swkim101/cspapers.org, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/cspapers-org

## Pinned environment

- Project commit: `92397bd6e2418b494f37b1c102c6706050b70480`
- Test commit: `92397bd6e2418b494f37b1c102c6706050b70480`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.9 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 8.9 | 5 | 5 | [run](https://argusic.com/run/f442ca48-31ab-45bf-8e13-bc4286023910) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go toolchain and Node >=20 not installed in container (no root, no apt)`
- 3 min: `npm install under Node 18 missed the optional native rolldown binding (@rolldown/binding-linux-x64-gnu missing), so vite build failed with 'Cannot find native binding'`
- 1 min: `index.html references /src/index.js, but the repo contains only src/index.jsx, so vite build failed with 'Failed to resolve /src/index.js'`
- 8 min: `The Semantic Scholar title dumps data/cstitles/batch-0..3 are not in the repository, so 'make index' panics ('open data/cstitles/batch-3: no such file') after indexing crawled papers, and 'npm run test:dupcheck' exits ENOENT on missing 'dat`
- `The API index build is incomplete: without data/cstitles the indexer dies mid-run, so db.cspapers.org covers only data present in the repo (2017-2026 crawled abstracts); no full index exists`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
