# jiratui

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/whyisdifficult/jiratui, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/jiratui

## Pinned environment

- Project commit: `0f8b318b15542cf97fd958bd403f32ab3f76394f`
- Test commit: `0f8b318b15542cf97fd958bd403f32ab3f76394f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 6.7 to 33.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.07 | 33.7 | 0 | 0 | [run](https://argusic.com/run/2b56c680-0b85-4582-9e85-65bcd8fc20c0) |
| 2 | pass with mocks | 92 | 0.5 | 6.7 | 1 | 1 | [run](https://argusic.com/run/f57fc042-18b7-434d-bdd3-a069922d912e) |

## What was observed on a clean machine

Attempt 2:

- 10 min: `Tree-sitter JSON language binding (tree_sitter_json) causes intermittent segfault when creating textual TextArea with language='json' during compose/set_document because the compiled C extension has an ABI mismatch with the host tree-sitter`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
