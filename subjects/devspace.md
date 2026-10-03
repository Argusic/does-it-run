# devspace

**Verdict: runs.** Argusic Score 90.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/devspace-sh/devspace, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/devspace

## Pinned environment

- Project commit: `8ff6260787edacfa2c0d30d1ff62358d36d482bc`
- Test commits: `8ff6260787edacfa2c0d30d1ff62358d36d482bc`, `531d3f973f09f7b6b4993c9ff58f80a4514b9ba2`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 4; wall time 4.1 to 27.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 13 | 14.2 | 1 | 0 | [run](https://argusic.com/run/604b5acb-47cd-44e2-9cca-ad48daab3a6f) |
| 1 | pass | 100 | 3 | 4.1 | 1 | 1 | [run](https://argusic.com/run/af907b2a-2b99-4845-af63-9916aca88202) |
| 2 | pass with mocks | 92 | 13 | 27.2 | 3 | 3 | [run](https://argusic.com/run/a8c701e4-f47b-4985-bdd0-285b6ea117b1) |
| 3 | pass | 90 | 15 | 16.4 | 2 | 1 | [run](https://argusic.com/run/00fb95ee-c416-4f3f-804b-a1bf0b349424) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `TestInitialSync in pkg/devspace/sync fails: "too many open files" from inotify traversal hitting container inotify limit (max_user_instances=128)`

Attempt 1:

- 1 min: `Node.js v18.19.1 below minimum required v22.19`

Attempt 2:

- 4 min: `go not installed; binary missing from PATH`
- 10 min: `pkg/devspace/sync: TestInitialSync timeout (too many open files)`
- `e2e tests: TestRunE2ETests fails (no Kubernetes cluster)`

Attempt 3:

- 2 min: `go: command not found in container`
- `e2e tests fail because no Kubernetes cluster is available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
