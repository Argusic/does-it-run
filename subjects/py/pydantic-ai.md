# pydantic-ai

**Verdict: runs.** Argusic Score 84.8 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pydantic/pydantic-ai, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/pydantic-ai

## Pinned environment

- Project commit: `5badf40a3c5156cdc893c7f9993f856d4de8a2bb`
- Test commit: `5badf40a3c5156cdc893c7f9993f856d4de8a2bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 18.6 to 51.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 1 | 51.2 | 3 | 0 | [run](https://argusic.com/run/074f8ae0-5540-42e4-8189-fd1c48e6c501) |
| 2 | pass | 97.5 | 0.4 | 18.6 | 8 | 7 | [run](https://argusic.com/run/ade5a505-47fc-47bd-9512-debd9d06d9f4) |

## What was observed on a clean machine

Attempt 1:

- `test_docs_examples fails with blockbuster BlockingError on os.path.samestat`
- `test_cli banner width assertion fails when version string is long`
- `2 realtime test_supports tests fail with blockbuster BlockingError`

Attempt 2:

- 1 min: `uv was not installed, so make install could not start`
- 1 min: `/usr/bin/time was absent`
- 1 min: `clai web -m test:test exited with 'Unknown model: test:test'`
- 4 min: `Initial all-extras pytest run produced numerous Prefect Blockbuster failures`
- 4 min: `Docs-example setup errors reported pyright exit code 247 after the cgroup recorded an OOM kill`
- 1 min: `Version probe assumed pydantic_evals and pydantic_graph expose __version__`
- 1 min: `uv pip check reported the Makefile's intentional --no-deps harness incompatibilities`
- 1 min: `Build command using rm -rf was rejected by command policy`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
