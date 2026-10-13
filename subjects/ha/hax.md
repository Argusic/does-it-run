# hax

**Verdict: runs with mocks.** Argusic Score 88 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OleksandrChekhovskyi/hax, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/hax

## Pinned environment

- Project commit: `6753f30e5f79c01b47925f690b90daaa4630b409`
- Test commit: `6753f30e5f79c01b47925f690b90daaa4630b409`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.9 to 6.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 88 | 18 | 6.9 | 5 | 4 | [run](https://argusic.com/run/f36ff3c9-674f-4f27-8fae-6207eb16dc1f) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `System lacks build deps (meson, ninja, libcurl-dev, jansson-dev) and install_deps.sh needs root (apt-get)`
- 2 min: `pkg-config rejected hand-written .pc files missing a Description field`
- 1 min: `curl headers resolved to system curl instead of extracted dev package`
- 4 min: `make lint failed: clang-format/clang-tidy missing (no root to apt-get)`
- 1 min: `tmux missing, so interactive REPL under the virtual display could not be exercised`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
