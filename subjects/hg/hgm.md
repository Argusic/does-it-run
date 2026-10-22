# HGM

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/metauto-ai/HGM, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/hgm

## Pinned environment

- Project commit: `013872d95da978483f5b540e531db063d23890da`
- Test commit: `013872d95da978483f5b540e531db063d23890da`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 31 to 31 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 40 | 31 | 7 | 7 | [run](https://argusic.com/run/2b965643-b34b-487b-9882-84470cb6707c) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `pip install -r requirements.txt left polyglot/benchmark.py unimportable: ModuleNotFoundError importlib_resources, and swe_bench/polyglot harnesses failed with ModuleNotFoundError: No module named 'swebench'`
- 5 min: `datasets import failed: ImportError: cannot import name 'BucketNotFoundError' from huggingface_hub.errors with huggingface-hub 1.4.1`
- 3 min: `swe_bench/harness.py and polyglot/harness.py crash before Docker: TypeError: harness() got an unexpected keyword argument 'num_samples'`
- 4 min: `hgm.py boot crashes in TS_sample with ValueError: attempt to get argmax of an empty sequence when Docker is absent (initial node has no utility_measures)`
- `Docker is required by run.sh (hgm.py) and both harnesses but the container has no docker binary/daemon and system packages cannot be installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
