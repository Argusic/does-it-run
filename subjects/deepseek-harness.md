# deepseek-harness

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deepseek-ai/deepseek-harness, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/deepseek-harness

## Pinned environment

- Project commit: `0a53fb55bea101816fa226bb964ae2bed71c343b`
- Test commit: `0a53fb55bea101816fa226bb964ae2bed71c343b`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run, no run possible
- Valid runs: 6; wall time 6.2 to 90.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 13.2 | 3 | 3 | [run](https://argusic.com/run/7c2eeae8-15ca-4456-b9df-463e90b7a112) |
| 1 | pass with mocks | 88 | 2.5 | 16.6 | 5 | 4 | [run](https://argusic.com/run/0f93e09d-1454-49aa-91dd-1cb4e4c4b428) |
| 1 | pass | 100 | 1 | 54.1 | 4 | 4 | [run](https://argusic.com/run/2b8e9826-79e4-438b-8ad3-f768408f78ed) |
| 2 | fail | 20 | 5 | 6.2 | 1 | 1 | [run](https://argusic.com/run/6f0ff226-9f66-4205-a513-27ef23880f2f) |
| 2 | timeout | none | 10 | 90.8 | 3 | 3 | [run](https://argusic.com/run/6d4c37f8-6631-467a-b61c-3c0cd3906134) |
| 3 | pass | 100 | 3 | 48 | 3 | 3 | [run](https://argusic.com/run/29f3b4a3-27d7-48f7-b904-a589383a5dc9) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js version 18.19.1 too old - project requires ^22.19.0 || >=24.0.0`
- 1 min: `TypeScript compilation errors - pi-ai package had new fields not in drift gates (thinking.budget, thinkingTokenBudgetField, allowedFallbackModels)`
- 1 min: `pnpm postinstall script failed - JSON import syntax not supported in Node 18`

Attempt 1:

- 1.5 min: `pnpm: command not found, and Node v18.19.1 does not satisfy required engines ^22.19.0 || >=24.0.0`
- 0.5 min: `Running the CLI from a workspace outside the repo failed: ERR_MODULE_NOT_FOUND 'tsx' (source launch resolves tsx relative to cwd)`
- 3 min: `10 test failures in packages/spill/spill-local (spill-local.spec.ts, loader-composition.spec.ts): sweep refused to delete aged files, warning 'skipped unsafe session directory'`
- 2 min: `spill-local 'keeps a file exactly at the boundary' fails ~50% of runs: utimesSync(cutoffMs/1000) float round-trip stores an mtime below cutoffMs, so the boundary file is treated as strictly older and deleted`
- 2 min: `packages/test-support/llm-mock-server 'formats an IPv6 listener as a valid base URL' fails with listen EADDRNOTAVAIL ::1`

Attempt 1:

- 2 min: `Node.js 18.19.1 in container, project requires ^22.19.0`
- 1 min: `pnpm not available in container PATH`
- 12 min: `spill-local cleanup tests: mkdirSync with umask 0002 creates mode 0775 dirs, but isTrustedDirectory rejects group-writable dirs`
- `IPv6 loopback unavailable in container`

Attempt 2:

- 5 min: `Node version constraint: container has v18.19.1 but project requires ^22.19.0 || >=24.0.0`

Attempt 2:

- 3 min: `Node.js v18.19.1 is too old (requires ^22.19.0 || >=24). Container only had v18.`
- `Full pnpm test suite does not complete within timeout , too large for container resources.`
- `10 pre-existing test failures in packages/spill/spill-local: cleanup sweep tests fail because expected file deletions do not occur. Root cause: the test's mocked tmpdir may interact incorrectly with container tmpdir sticky-bit/writable-by-o`

Attempt 3:

- 10 min: `Container umask 0002 causes mkdirSync with { recursive: true } (no explicit mode) to create group-writable (0775) directories. The sweep's isTrustedDirectory check requires mode & 0o22 === 0, rejecting them. Affected: 9 tests in spill-local`
- 5 min: `Boundary test (keeps a file exactly at the cutoff) is flaky because utimesSync stores second-level precision but Date.now() has millisecond precision. The sweep comparison mtimeMs >= cutoffMs can fail when sub-millisecond rounding changes t`
- 2 min: `IPv6 loopback (::1) is unavailable in this container, causing listen EADDRNOTAVAIL on the IPv6 listener test.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
