# forest

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dromara/forest, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/forest

## Pinned environment

- Project commit: `52d68e974c54229ea2ce5daf9392aaa3b621938f`
- Test commit: `52d68e974c54229ea2ce5daf9392aaa3b621938f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 33.3 to 87.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | 10 | 87.9 | 3 | 3 | [run](https://argusic.com/run/2f460413-94bf-48c8-818f-13b13f0f43c1) |
| 2 | pass | 100 | 8 | 33.3 | 6 | 6 | [run](https://argusic.com/run/62f523c8-c7b1-4c16-9de4-30c78af4a02b) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `maven-surefire-plugin 2.18.1 in pom.xml had skipTests=true and used an outdated version that caused forked test processes to hang on pool tests (CountDownLatch) and SSE tests`
- `TestUploadClient.testCancelUploadFile had 3 pre-existing failures (expected true, got false) on okhttp3 backend with all 3 JSON converters`
- 8 min: `No Java or Maven installed in base container`

Attempt 2:

- 2 min: `Java 8 runtime not found in container`
- 1 min: `Maven not installed`
- 1 min: `maven-surefire-plugin had hardcoded skipTests=true preventing test execution`
- `forest-jakarta-xml module requires Java 17 (maven.compiler.target=17)`
- `TestGenericForestClient, TestDownloadClient, TestUploadClient, TestAsyncGetClient etc. hang/timeout due to async coroutine mode or real network calls`
- `forest-spring tests fail with XML schema validation error (cvc-complex-type.2.4.c) due to strict Xerces in JDK 17`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
