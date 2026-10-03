# UptimeKit-CLI

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/abhixdd/UptimeKit-CLI, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/uptimekit-cli

## Pinned environment

- Project commit: `616373ef769dfca28e6ac761d17e600ce38a305c`
- Test commit: `616373ef769dfca28e6ac761d17e600ce38a305c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 8.7 to 18.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 8.7 | 2 | 2 | [run](https://argusic.com/run/8654bd0d-c00a-4bba-85ef-72c33868a97c) |
| 2 | pass with mocks | 92 | 20 | 18.5 | 3 | 3 | [run](https://argusic.com/run/5b1a4be9-8a18-4f62-bd1f-110f136beabd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Ink v6 dependency string-width@8.1.0 uses ES2024 /v regex flag unsupported in Node.js v18`
- 1 min: `Snapshot tests had whitespace mismatches after Ink downgrade`

Attempt 2:

- 3 min: `Node.js 18 cannot parse '/v' regex flags used by ink@6.5.1, string-width@8.1.0, cli-truncate@5.1.1 , all require Node >=20`
- 2 min: `better-sqlite3 native addon segfaults under Node 22 because it was compiled for Node 18's ABI`
- 3 min: `'edit' command's Zod schema had 'retries: z.number().positive()' which rejects 0, the default retries value, breaking every edit operation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
