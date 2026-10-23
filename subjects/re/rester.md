# RESTer

**Verdict: runs.** Argusic Score 55 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/frigus02/RESTer, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/rester

## Pinned environment

- Project commit: `235ebd2063ebbd2bee54f8e63c190da5f18b7554`
- Test commit: `235ebd2063ebbd2bee54f8e63c190da5f18b7554`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 9.8 to 15.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 15.6 | 0 | 0 | [run](https://argusic.com/run/0a2851ac-2a50-42d0-8ce8-2e7375ae4413) |
| 2 | pass | 90 | 10 | 9.8 | 4 | 2 | [run](https://argusic.com/run/b641e36f-587b-43b9-a4df-66a56d71bb0d) |

## What was observed on a clean machine

Attempt 2:

- 4 min: `System Node is v18 but project requires >=24 and yarn (>=1) is not installed`
- 3 min: `No Firefox binary on system, and the e2e suite locates Firefox only via firefox.Channel.DEV.locate() (PATH lookup on Linux)`
- 2 min: `yarn start (watch mode) fails with EMFILE: too many open files due to container inotify max_user_instances=128 while watching node_modules; unfixable without root sysctl`
- 1 min: `One jest --testNamePattern invocation transiently failed with 'Could not locate Firefox' under PATH pollution from the geckodriver globalSetup (semicolon-delimited PATH); full-suite runs were consistently green`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
