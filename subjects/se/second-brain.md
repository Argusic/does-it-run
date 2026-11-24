# second-brain

**Verdict: runs.** Argusic Score 94 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/henrydaum/second-brain, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/second-brain

## Pinned environment

- Project commit: `d79ca2e1859a15beccde8b9927a0f77e36e136c4`
- Test commit: `d79ca2e1859a15beccde8b9927a0f77e36e136c4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 35.2 to 51 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 51 | 51 | 5 | 4 | [run](https://argusic.com/run/277fcb5a-ef2b-4667-8a1b-ebf01ef3204f) |
| 2 | pass with mocks | 92 | 0.5 | 35.2 | 3 | 3 | [run](https://argusic.com/run/a1266679-7f2f-431f-8b40-5e57a6ed3bbd) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js 18 too old for web UI (requires ^20.19.0 or >=22.12.0). Vite fails with SyntaxError on node:util.styleText.`
- 8 min: `Stale orphan LISTEN socket on port 8787 from prior test processes blocks HTTP frontend. No process holds the socket but it persists in LISTEN state.`
- 3 min: `Plugin watcher fails with inotify instance limit reached (EMFILE, errno 24) when orphaned guest.child subprocesses accumulate from test runs.`
- 2 min: `REPL frontend fails with the console is closed in non-interactive environment (no TTY available).`
- `2 pre-existing test failures in test_sandbox_processes.py: test_starting_a_process_asks_unless_something_vouches_for_it[ls-proc.run] and [ls-proc.start] - sandbox now classifies ls as safe but tests expect it to be unsafe.`

Attempt 2:

- 3 min: `cron_descriptor 2.3.5 changed output format (added AM/PM)`
- 3 min: `test_sandbox_processes expected ls to be unsafe but read-only recognizer marks it safe`
- 1 min: `Node.js 18.19.1 is below required 20.19.0 for frame_ui package`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
