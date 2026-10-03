# chrome-devtools-mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ChromeDevTools/chrome-devtools-mcp, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/chrome-devtools-mcp

## Pinned environment

- Project commit: `b2007ab86639a0ae4e4370484561158773112b93`
- Test commit: `b2007ab86639a0ae4e4370484561158773112b93`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 42 to 51.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/b2072085-dd8c-42c8-ada2-97967f155e23) |
| 1 | pass | 100 | 44 | 51.2 | 6 | 6 | [run](https://argusic.com/run/6fcb4309-27e4-40a6-83ce-749b37139cde) |
| 2 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/6423a0b3-b4df-4ca5-8c77-a16339e59aa3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 on host, project requires >=22.12.0. Downloaded and used Node.js v22.13.0 from binary tarball.`
- 2 min: `prepare.ts is a TypeScript file that cannot be run directly by Node.js without a TS runner.`
- 2 min: `post-build.ts has the same issue as prepare.ts.`
- 2 min: `Chrome not installed. Puppeteer browsers install failed: missing unzip and empty cache directory.`
- 1 min: `Chrome sandbox prevents launch in container without --no-sandbox.`
- 5 min: `Chrome not found at /opt/google/chrome/chrome (system path), failing e2e tests.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
