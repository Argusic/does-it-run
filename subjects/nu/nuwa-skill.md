# nuwa-skill

**Verdict: runs with mocks.** Argusic Score 84.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alchaincyf/nuwa-skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/nuwa-skill

## Pinned environment

- Project commit: `fe0374687037c4cc51a65c1e0c145afe2981dc69`
- Test commit: `fe0374687037c4cc51a65c1e0c145afe2981dc69`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 11.2 to 18.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 16 | 18.6 | 2 | 1 | [run](https://argusic.com/run/783b34b9-085b-4129-8d1e-7b9cccf378c5) |
| 2 | pass with mocks | 92 | 1 | 11.2 | 2 | 2 | [run](https://argusic.com/run/8f696377-b643-4e23-af13-0537937feaa6) |
| 3 | pass with mocks | 80 | 14 | 13.6 | 5 | 2 | [run](https://argusic.com/run/e27f646b-9a30-445c-821c-aae81af16b09) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `npx skills add failed: Node v18 lacks node:util styleText export (needs >=22.20)`

Attempt 2:

- 3 min: `quality_check.py check_honest_boundary only counted '-'/'*' bullets, but examples use numbered lists (1., 2., ...) causing 13 false failures`
- 2 min: `quality_check.py check_tensions regex did not match 'vs' separator used in tension items`

Attempt 3:

- 1 min: `npx skills add failed: Node.js v18 too old (needs v22)`
- 1 min: `pip3 install blocked by PEP 668 external packages policy`
- `merge_research.py: 4 of 15 example dirs use nonstandard research file naming (not 01-06 prefix)`
- `quality_check.py: 13 of 15 example skills fail 'honest boundary >= 3 items' check (pre-existing content gap)`
- `srt_to_transcript.py -o flag not implemented (uses positional arg only)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
