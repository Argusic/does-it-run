# shopping-cart

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shashirajraja/shopping-cart, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/shopping-cart

## Pinned environment

- Project commit: `30fcead06d85c04a93b277d696b9efaa279673b7`
- Test commit: `30fcead06d85c04a93b277d696b9efaa279673b7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.1 to 10.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 10.1 | 6 | 6 | [run](https://argusic.com/run/3e064399-1ec2-4f09-82fc-38f62cf0586b) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No JDK or Maven installed in container`
- 1 min: `No MySQL database available`
- 1 min: `H2 SQL reserved keyword 'user' caused syntax errors`
- 0.5 min: `Queries referenced schema prefix 'shopping-cart'.product which doesn't exist in H2`
- 0.5 min: `Search was case-sensitive (H2 LIKE != MySQL LIKE behavior)`
- 0.5 min: `Add to cart did not insert new cart items, only updated existing ones`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
