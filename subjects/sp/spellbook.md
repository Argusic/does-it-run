# spellbook

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/majiayu000/spellbook, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/spellbook

## Pinned environment

- Project commit: `414b597ec113b9c8d37c8de912ef80f92d9ad2f3`
- Test commit: `414b597ec113b9c8d37c8de912ef80f92d9ad2f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 11.8 to 13 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 11.8 | 0 | 0 | [run](https://argusic.com/run/c70609b4-8e58-4574-b282-1a00b5ea58ce) |
| 2 | pass | 100 | 35 | 13 | 3 | 3 | [run](https://argusic.com/run/228cdee5-aef1-4303-aa5e-62e21138f8e3) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Missing PyYAML dependency: 7 tests failed to collect with ModuleNotFoundError for 'yaml'`
- 1 min: `Out-of-date generated registry files (skills.json, tags.json, skill-registry.md, skills.html) fail validation`
- 2 min: `install.sh had an inline Python parser that rejected upstream frontmatter format (compatibility string + metadata dict), plus banner count mismatch (112 vs 109)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
