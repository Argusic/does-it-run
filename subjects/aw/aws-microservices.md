# aws-microservices

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/awsrun/aws-microservices, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/aws-microservices

## Pinned environment

- Project commit: `b96acb04709dd6386d03fce709b5ca9bdd7b67ba`
- Test commit: `b96acb04709dd6386d03fce709b5ca9bdd7b67ba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7.8 to 21.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 8.5 | 7.8 | 2 | 2 | [run](https://argusic.com/run/1879c7ba-ba1d-47c7-a836-8f84ab4fdf59) |
| 2 | pass | 100 | 12 | 21.9 | 3 | 3 | [run](https://argusic.com/run/515b33a2-a7f4-4471-91a6-679362f31c92) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Docker not available for NodejsFunction bundling`
- 2 min: `Missing @aws-sdk packages for esbuild bundling resolution`

Attempt 2:

- 8 min: `cdk synth failed: NodejsFunction requires Docker for esbuild bundling, but Docker is not in the container`
- 2 min: `Lambda JS source uses ES import syntax not loadable via require() in CJS mode`
- 3 min: `DynamoDB and EventBridge client constructors need explicit endpoint for local/Dynalite endpoints`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
