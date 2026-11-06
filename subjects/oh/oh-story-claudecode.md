# oh-story-claudecode

**Verdict: runs.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zenstory-ai/oh-story-claudecode, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/oh-story-claudecode

## Pinned environment

- Project commit: `4a50d5583590eb7f207037e35136c1168bc02201`
- Test commit: `4a50d5583590eb7f207037e35136c1168bc02201`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.9 to 20.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 15.9 | 1 | 1 | [run](https://argusic.com/run/2c65353b-2e34-4bcd-912d-3ebd4380e319) |
| 2 | pass | 96 | 22 | 20.1 | 5 | 4 | [run](https://argusic.com/run/6de2537c-ffc4-42f1-a853-4f1b7f748c7d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test-prose-net-parity.sh failed because the "node absent" test scenario still had node in PATH (/usr/bin), so node was never truly unavailable; only "/usr/bin:/bin" were in PATH`

Attempt 2:

- 4 min: `npx skills add requires Node >=22.20 but container has node v18.19.1 (node:util.styleText missing)`
- 2 min: `npx skills add -g (global) reports 'PromptScript does not support global skill installation' for all 14 skills; global install path fails`
- 25 min: `scripts/test-prose-net-parity.sh FAIL: 'node 缺席时追踪门未 fail-open' on hosts where node lives in /usr/bin; empty PATH prefix cannot shadow /usr/bin/node so test never exercised fail-open path`
- `scripts/test-scan-runtime.js CDP-owner-verification subtest requires lsof/ss/fuser + Chrome, both absent in container; subtest not verified`
- 2 min: `Playwright installed browsers initially absent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
