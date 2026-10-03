# gocd

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gocd/gocd, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/gocd

## Pinned environment

- Project commit: `9a49867bc65426e55bb6ce8aa17cc2afc9862dd4`
- Test commit: `9a49867bc65426e55bb6ce8aa17cc2afc9862dd4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 42 to 42 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 41 | 42 | 5 | 5 | [run](https://argusic.com/run/5eb05019-8ef9-40fa-b935-a12e0236a809) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No Java JDK found in container`
- 1 min: `Gradle toolchain requires JDK 25 but auto-provisioning disabled`
- 1 min: `JRuby initializeRailsGems fails with 'Could not create JVM' due to --sun-misc-unsafe-memory-access=allow flag not supported by JDK 21`
- `SCM binary tests fail: svn, hg, p4, ant not installed (no root)`
- `JettyWorkDirValidatorTest.shouldSetJettyHomeAndBasePropertyIfItsNotSet fails - pre-existing test design issue with Mockito mock vs System.setProperty`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
