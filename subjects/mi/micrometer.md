# micrometer

**Verdict: runs.** Argusic Score 54 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/micrometer-metrics/micrometer, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/micrometer

## Pinned environment

- Project commit: `85e64cfa1c4d0fbb2b4accd468c2dc438c24a1e8`
- Test commit: `85e64cfa1c4d0fbb2b4accd468c2dc438c24a1e8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 29.9 to 83.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 83.7 | 0 | 0 | [run](https://argusic.com/run/2d5eba56-cbaa-469a-8f60-785af52a01fb) |
| 2 | pass | 88 | 32 | 29.9 | 5 | 2 | [run](https://argusic.com/run/be9b6d85-f61e-414b-ad33-5337b1eabbef) |

## What was observed on a clean machine

Attempt 2:

- 9 min: `No Java JDK in container - JAVA_HOME not set, java command not found`
- 20 min: `nebula.publish-verification plugin substitutes project(':micrometer-core') with external Maven Central artifact micrometer-core:1.17.0, causing NoSuchMethodError: DefaultMeterObservationHandler.builder() at test runtime`
- `DynatraceMeterRegistryTest.shouldTrackPercentilesWhenDynatraceSummaryInstrumentsNotUsed fails - LongTaskTimer percentile export wrong values`
- `StatsdMeterRegistryPublishTest.resumeSendingMetrics_whenServerIntermittentlyFails timeout`
- `TimedHandlerTest (jetty12) - expected 2 request count got 1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
