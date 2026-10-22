# terminal

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/browser-use/terminal, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/terminal

## Pinned environment

- Project commit: `16cdd3ac47261292d88f410abb1f0234577850ce`
- Test commit: `16cdd3ac47261292d88f410abb1f0234577850ce`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 22.1 to 40.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 22.1 | 0 | 0 | [run](https://argusic.com/run/0bdacd56-9c09-4f84-b21c-02abcfd640d0) |
| 2 | pass | 100 | 17 | 40.1 | 6 | 6 | [run](https://argusic.com/run/e1af0145-a0ca-43a9-8c21-1e594cc6a843) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `cargo/rustc not installed in container`
- 1 min: `uv not installed`
- 6 min: `22 browser-use-browser test failures: stale 15s->30s initial-wait assertion poisoned global ENV_LOCK causing cascading env-lock-poisoned panics`
- 5 min: `6 browser-use-agent test failures: 5 prompt tests asserted removed phrases; 1 recovery test asserted obsolete architecture`
- 2 min: `1 browser-use-tui test failure: OPENROUTER_API_KEY set in container broke auth-first assertion`
- 1 min: `tmux missing for scripts/verify-terminal-ui.sh real-terminal smoke (exit 2)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
