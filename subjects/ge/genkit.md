# genkit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/genkit-ai/genkit, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/genkit

## Pinned environment

- Project commit: `6b34d5fe691002a217e11228b85979f58664288b`
- Test commit: `6b34d5fe691002a217e11228b85979f58664288b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 25.9 to 64.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 25.9 | 4 | 4 | [run](https://argusic.com/run/b0775336-f11e-4203-baa5-5c0f4a33066e) |
| 2 | pass | 100 | 64 | 64.9 | 5 | 5 | [run](https://argusic.com/run/1ad686d5-8529-4636-8b8f-6cb48efeea6d) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `pnpm node-linker default (isolated) didn't create .bin symlinks, causing 'npm-run-all: not found'`
- 3 min: `@types/request transitively referenced tough-cookie CookieJar type which was renamed in tough-cookie v6, causing tsc to fail on core build`
- `core test: 1 pre-existing flaky failure in bidi-action_test.ts (unhandledRejection race)`
- `genkit test: 1 pre-existing failure in mockModel agent handoff test`

Attempt 2:

- 30 min: `JS/ai package: 172 tests fail due to globalThis.crypto.randomUUID() being undefined in some tsx loader contexts on Node.js 18 (requires Node.js 20+ per docs)`
- `JS/core package: 1 test failure (bidi-action: stream race condition)`
- `JS/genkit package: 1 test failure (agent handoff test uses crypto.randomUUID)`
- `Python/core: 1 test failure (test_serves_on_ipv6_loopback - IPv6 not available in container)`
- `Go SDK not available (no Go compiler in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
