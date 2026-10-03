# oh-my-agent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/first-fluke/oh-my-agent, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/oh-my-agent

## Pinned environment

- Project commit: `c7417362f8f9997567ca71e614b57758fe093c9a`
- Test commit: `c7417362f8f9997567ca71e614b57758fe093c9a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 10.7 to 52.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 10.7 | 4 | 4 | [run](https://argusic.com/run/07f067ef-5363-4145-a7e8-60c17b5efb2c) |
| 2 | pass | 100 | 8 | 52.6 | 3 | 3 | [run](https://argusic.com/run/0361610b-1e39-4241-b8bb-75e5be82d41f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node v18 is too old (requires >=26)`
- 1 min: `bun not found`
- 2 min: `mawk doesn't support Unicode bracket expressions in filter-test-output.sh`
- 1 min: `/tmp/.agents directory (from OMA hooks) causes test backup path collisions in opt.test.ts`

Attempt 2:

- 2 min: `Node.js v18.19.1 too old for vitest 4.x (needs node:util.styleText from node >=26). Bun install succeeded but vitest died at startup.`
- 3 min: `mawk cannot handle multi-byte UTF-8 chars inside awk bracket expressions [✓√✔] in filter-test-output.sh. 12 tests in filter-test-output.test.ts had 1 failure.`
- 10 min: `transport.test.ts used cwd: "/tmp" which triggered state-boundary hook creating /tmp/.agents/state/sessions/. This contaminated backup.test.ts findProjectRoot (walked up tmpdirs and wrongly found /tmp as project root). Caused backup.test.ts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
