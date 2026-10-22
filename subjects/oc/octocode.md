# octocode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Muvon/octocode, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/octocode

## Pinned environment

- Project commit: `9c7f4b96675b6abcee5f25098c663b4f1a9bec15`
- Test commit: `9c7f4b96675b6abcee5f25098c663b4f1a9bec15`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 46.8 to 46.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 44 | 46.8 | 3 | 3 | [run](https://argusic.com/run/259e6734-4296-4bc8-a652-b33e278e0035) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Rust toolchain in container (cargo/rustc not found).`
- 2 min: `Full-feature build requires protoc, which was absent.`
- 1 min: `unzip binary not present in container.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
