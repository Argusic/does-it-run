# jquick-curl

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dromara/jquick-curl, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/jquick-curl

## Pinned environment

- Project commit: `35f8d038bf17baa318d901568e680c187530b563`
- Test commit: `35f8d038bf17baa318d901568e680c187530b563`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.2 to 8.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 8.2 | 8 | 8 | [run](https://argusic.com/run/d3195598-1c5f-44b5-9778-53e60b6412c1) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No java, javac, or mvn was installed, so the documented Maven build could not start.`
- 1 min: `Maven reported JAVA_HOME was not defined correctly after unpacking.`
- 4 min: `Initial mvn test ran 33 tests with 22 errors: 21 null responses from the missing localhost:8080 API and one 'Expected URL scheme ... userId' parser failure.`
- 3 min: `Multipart upload tests failed because fixtures used nonexistent Windows paths D:\test, and downloads wrote to d:/test.`
- 2 min: `Processor and direct visitor tests threw ClassCastException casting JQuickCurlResponseBody to JResult.`
- 3 min: `JCurlCommandProcessorTest failed with 'java.lang.IllegalArgumentException: timeout too large' in OkHttp.`
- 2 min: `mvn clean install failed at maven-gpg-plugin because gpg was not installed.`
- 2 min: `The first external Python mock exited when its parent shell ended, so tests still received connection refused.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
