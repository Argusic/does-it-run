# flask

**Verdict: runs.** Argusic Score 88.6 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pallets/flask, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/flask

## Pinned environment

- Project commit: `d318b683471101618febed18996405ad26462110`
- Test commit: `d318b683471101618febed18996405ad26462110`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 7; wall time 1.1 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 2.8 | 1 | 1 | [run](https://argusic.com/run/0032726c-3af9-45c8-84bc-4238ae8af441) |
| 1 | fail | 20 | 15 | 2.1 | 4 | 4 | [run](https://argusic.com/run/e074089f-7f2a-4239-9bcf-46ceb81564ad) |
| 1 | pass | 100 | 2 | 1.5 | 0 | 0 | [run](https://argusic.com/run/49866b83-1a40-4c15-9fb9-3af2f86fb238) |
| 1 | pass | 100 | 0.15 | 1.7 | 0 | 0 | [run](https://argusic.com/run/f8acb2d0-f47a-47eb-a4e8-b279f51e5717) |
| 1 | pass | 100 | 1 | 2 | 0 | 0 | [run](https://argusic.com/run/9dc53799-a195-4690-b917-8ded49cd7cd7) |
| 1 | pass | 100 | 5 | 1.1 | 1 | 1 | [run](https://argusic.com/run/1e5c3b16-3aef-47b7-817a-104ee3060d90) |
| 2 | pass | 100 | 4 | 1.5 | 0 | 0 | [run](https://argusic.com/run/c414347a-2f18-4ecc-a06c-8996895364c6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Container missing pip/venv support: python3-venv not installed`

Attempt 1:

- 3 min: `pip module not found - attempted 'pip', 'pip3', and 'python3 -m pip'`
- 4 min: `Virtual environment creation failed: ensurepip module not available and python3.12-venv package not installed`
- 4 min: `apt-get permission denied on /var/lib/apt/lists/lock - running as unprivileged 'runner' user`
- 4 min: `setuptools, distutils, and other Python packaging tools not available`

Attempt 1:

- 1 min: `Flask async extra not installed, required for async view tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
