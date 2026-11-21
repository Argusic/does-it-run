# openharness

**Verdict: runs.** Argusic Score 91 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/autonomous-ai/openharness, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openharness

## Pinned environment

- Project commit: `e7736e268fe6b730eb38f92b793fa746564dfb25`
- Test commit: `e7736e268fe6b730eb38f92b793fa746564dfb25`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 47.6 to 54.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 45 | 47.6 | 7 | 7 | [run](https://argusic.com/run/ea4195d9-1bb1-4647-b9d0-a56e883020eb) |
| 2 | pass with mocks | 82 | 58 | 54.6 | 8 | 4 | [run](https://argusic.com/run/a3b9feee-4edb-4546-8ed3-5b047676676a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `sqlite3 CLI not on PATH , 9 tests in opencode/hermes/devin spec failed because the sqlite3 CLI reader path couldn't find the binary`
- 2 min: `umask 0002 caused mkdtempSync to create group-writable temp dirs (0775) which secureStateDirectory rejects`
- 5 min: `Test PATH /usr/bin:/bin contains /usr/bin/node (v18), so dshNodeFallback (which checks 'command -v node') never appends the managed runtime, causing 2 tests to fail`
- 5 min: `lsof not available in container , support.spec.ts processView test could not list open files of the current process`
- 3 min: `machineList.spec.ts mtimeMs check failed because filesystem writes happened within the same millisecond`
- 5 min: `loginForceRace.spec.ts timed out because tsx transpilation startup was too slow in the container`
- 3 min: `dsh/install.spec.ts doctor timeout test exceeded 5s default vitest timeout because the 'sleep 30' subprocess kill-then-SIGKILL grace period took too long`

Attempt 2:

- 3 min: `Node 18.19.1 shipped in container, project needs >=20`
- 10 min: `tmux not installed; project requires it for agent lifecycle (tmux sessions)`
- 3 min: `sqlite3 CLI not installed; needed for SQLite engine conversation store fallback (Node <22)`
- `No root access; cannot use apt install for any dependency`
- `test: support.spec.ts 'lists the real machine' fails - cannot find vitest process's own open file in /proc`
- `test: engineLaunch.spec.ts 'DSH prelude reaches engine PATH' - expects runtime bin dir in PATH but test dirs mismatch the fixture`
- `test: authCommand, cliCommand, loginForceRace, backendSocket time out - these tests expect loopback HTTP/WebSocket servers for SSO flow and do not complete without network`
- `test: e2ee/relayLink.spec.ts, e2ee/manager.test.ts, gridReads.spec.ts, terminalStreamManager.spec.ts, orchestrator/service.spec.ts and dsh/shell.spec.ts fail - timeouts or expectations requiring full daemon`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
