# zookeeper

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/zookeeper, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/zookeeper

## Pinned environment

- Project commit: `b9818714f4790347c27f37fd49739a91b46c8e5e`
- Test commit: `b9818714f4790347c27f37fd49739a91b46c8e5e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 32.3 to 32.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 32.3 | 2 | 2 | [run](https://argusic.com/run/1fe8174c-54b3-406e-bc35-4296e413a212) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Java or Maven in container (no root for apt)`
- 0.5 min: `C client module (zookeeper-client-c) requires autoreconf (not available)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
