# skills

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/google/skills, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/run/8405f33c-bf9c-4bed-a684-686a47b58e16

## Pinned environment

- Project commit: `f004524de788065fcfbbdb8b07ee69493c6ec190`
- Test commit: `f004524de788065fcfbbdb8b07ee69493c6ec190`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 7.5 to 9.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 9.5 | 5 | 5 | [run](https://argusic.com/run/8405f33c-bf9c-4bed-a684-686a47b58e16) |
| 2 | pass | 100 | 29 | 7.5 | 4 | 4 | [run](https://argusic.com/run/fdcffb3f-057c-42ca-bad9-f4e099144679) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npx skills add google/skills requires Node >=22.20.0, container has v18.19.1`
- 2 min: `assemble_widget_proto_test.py: absltest.TestCase.create_tempdir() fails with unparsed flags`
- 2 min: `fetch_terraform_template_test.py: absl flags accessed before parsing`
- 2 min: `list_terraform_templates.py: DuplicateFlagError when imported alongside sibling module`

Attempt 2:

- 1 min: `Missing Python dep promql-parser in validate_promql.py`
- 2 min: `absl flags collision in fetch_terraform_template_test.py and list_terraform_templates_test.py when running together under pytest`
- 1 min: `absl flags unparsed in assemble_widget_proto_test.py (test_tmpdir flag)`
- 3 min: `npx skills CLI requires Node >=22 but container has Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
