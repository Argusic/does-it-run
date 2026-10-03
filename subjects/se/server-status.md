# server-status

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/server-status-project/server-status, licensed Apache-2.0, written in PHP.

Evidence and recordings: https://argusic.com/subject/server-status

## Pinned environment

- Project commit: `4e4eb24305533160c8e01366a6935914d6846839`
- Test commit: `4e4eb24305533160c8e01366a6935914d6846839`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 26.6 to 38.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 37 | 38.4 | 4 | 4 | [run](https://argusic.com/run/4ab2f3b7-e4ec-4b31-a83c-5612f6dadc1b) |
| 2 | pass | 100 | 27 | 26.6 | 5 | 5 | [run](https://argusic.com/run/b383a9d4-dc87-4b66-98d1-6f488ae4eae3) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `No PHP runtime in environment`
- 15 min: `Missing MySQL/MariaDB database server`
- 5 min: `Missing PHP gettext extension`
- 6 min: `Duplicate constant definition warnings across multiple PHP files`

Attempt 2:

- 5 min: `PHP not installed in container`
- 8 min: `MariaDB not installed in container`
- 1 min: `Session save path missing`
- 2 min: `PHP config had placeholder values`
- 2 min: `Database settings table empty caused null URLs in template`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
