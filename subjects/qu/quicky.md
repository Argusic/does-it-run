# quicky

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alohe/quicky, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/quicky

## Pinned environment

- Project commit: `0fc73771ee8e71cd9b388abea2d3dedbc6645b0c`
- Test commit: `0fc73771ee8e71cd9b388abea2d3dedbc6645b0c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.8 to 89.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 89.8 | 0 | 0 | [run](https://argusic.com/run/e556feb2-5836-40a3-89c1-4e60c948039d) |
| 2 | pass | 100 | 0.1 | 6.8 | 3 | 3 | [run](https://argusic.com/run/61cf244b-e728-45a3-9753-033f61995369) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `Global npm install (npm install -g .) failed with EACCES - no root access`
- 2 min: `'init' command tries sudo apt install for nginx, certbot, git, curl, and sudo npm install -g pm2 - all fail without root`
- 1 min: `Interactive inquirer prompts fail in non-TTY environment for deploy, webhooks, and domains commands`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
