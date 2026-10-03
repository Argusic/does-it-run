# waha

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/devlikeapro/waha, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/waha

## Pinned environment

- Project commit: `55a7d78e3feaf24280fd2a16177ad6187202ea00`
- Test commit: `55a7d78e3feaf24280fd2a16177ad6187202ea00`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 61.7 to 61.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 61.7 | 7 | 7 | [run](https://argusic.com/run/72e203bc-d527-4039-b8e6-d903b85163cc) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18 installed, project requires v22+ (v24 per .nvmrc)`
- 5 min: `Yarn 3 shipped by corepack, project needs yarn 4.17.1 for berry PnP compatibility`
- 2 min: `8 unit tests in session.abc.test.ts failed: buildSession() missing media config parameter`
- 15 min: `2 unit tests in PhoneNumbersCacheRepository.test.ts failed: knex+sqlite3 Date handling inconsistency , stores epoch ms as number for onConflict merge but Date.toISOString() string for plain insert, causing TTL comparison to always pass and`
- 8 min: `2 test suites (PixMessage, message.ack.utils) fail to load: @adiwajshing/baileys is ESM-only, Jest won't transform it through transformIgnorePatterns`
- 5 min: `dist/vendor/esm.js compiled await import() to require() which cannot load ESM Baileys`
- 2 min: `All other source files import @adiwajshing/baileys directly; compiled require() calls fail on ESM module`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
