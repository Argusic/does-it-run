# api-gateway

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/membrane/api-gateway, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/api-gateway

## Pinned environment

- Project commit: `ca74996ec7aab3114249b3ee997296ebc41cbfcd`
- Test commit: `ca74996ec7aab3114249b3ee997296ebc41cbfcd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 7.3 to 30 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 30 | 3 | 3 | [run](https://argusic.com/run/9923b89e-e324-4ab4-9aab-8fb0097bc32f) |
| 2 | pass with mocks | 92 | 8 | 7.3 | 4 | 4 | [run](https://argusic.com/run/dbf89e8c-42d7-4a3a-8931-b4563161eb8c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `java/mvn not found in container`
- 1 min: `mvn test -pl core: Http2ClientServerTest.testStreamInfoProperlyClosed failed (expected CLOSED, got HALF_CLOSED_LOCAL)`
- 2 min: `tar could not extract membrane zip and membrane.sh lacked +x after extraction`

Attempt 2:

- 3 min: `No Java or Maven in container (java: not found, mvn: not found); no system install allowed`
- `unzip binary not available to extract distribution zip`
- 1 min: `Gateway exited immediately after 'up and running' because the launching shell reaped the background process (curl returned 000)`
- 1 min: `My hand-written conf/apis.yaml failed to parse ('Expected object' at empty '- return:'), due to a transcription error in the template/return block`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
