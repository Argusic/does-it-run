# tsk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/smarzban/tsk, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/tsk

## Pinned environment

- Project commit: `ade0385fa49f28035c35dc846ce90158c4117207`
- Test commit: `ade0385fa49f28035c35dc846ce90158c4117207`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.4 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 6.4 | 2 | 2 | [run](https://argusic.com/run/6a10ecdb-4ad0-47c0-96fb-32db074d9c0a) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `No Rust toolchain in container (no root); rustup absent`
- 10 min: `cargo test: cli_router_process::update_directs_a_homebrew_binary_to_brew_without_a_path_lookup failed once with ETXTBSY (Text file busy)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
