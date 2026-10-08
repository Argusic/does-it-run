# obsei

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/obsei/obsei, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/obsei

## Pinned environment

- Project commit: `cb61269ef91647e5334f0b67aaa0467802c5369a`
- Test commit: `cb61269ef91647e5334f0b67aaa0467802c5369a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.5 to 12.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 40 | 12.5 | 4 | 4 | [run](https://argusic.com/run/b2dbfb5d-bd6c-4ecb-b679-a038c1d5c1ab) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `NLTK resource 'punkt_tab' not found - text cleaners and splitters fail`
- 5 min: `Missing optional dependencies for import tests (pyfacebook, elasticsearch, app-store-reviews-reader, etc.)`
- 3 min: `TransformersNERAnalyzer fails with TypeError: grouped_entities removed in transformers v5`
- 5 min: `TranslationAnalyzer fails with KeyError: translation task removed in transformers v5`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
