# claude-for-legal

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/anthropics/claude-for-legal, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-for-legal

## Pinned environment

- Project commit: `4a6c651889c97cc9140580363c73e0eb17379c2b`
- Test commit: `4a6c651889c97cc9140580363c73e0eb17379c2b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.7 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 5.8 | 0 | 0 | [run](https://argusic.com/run/b368eb8e-73e8-4186-8bba-c892f19497fe) |
| 2 | pass | 100 | 3.5 | 5.7 | 2 | 2 | [run](https://argusic.com/run/c04be44c-4dc2-4a80-84d7-27051dff4943) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `managed-agent-cookbooks/diligence-grid/subagents/extractor.yaml output_schema has YAML null instead of string "null" in value.type array, breaking jsonschema validation`
- 1 min: `System python3 missing pyyaml and jsonschema modules; scripts/test-cookbooks.sh calls unqualified python3 and fails without venv`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
