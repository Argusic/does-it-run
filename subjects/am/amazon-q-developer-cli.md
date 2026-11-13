# amazon-q-developer-cli

**Verdict: runs.** Argusic Score 92.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aws/amazon-q-developer-cli, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/amazon-q-developer-cli

## Pinned environment

- Project commit: `15cc8f3cd18c4272925ce1c7053268eedff1ea0a`
- Test commit: `15cc8f3cd18c4272925ce1c7053268eedff1ea0a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 6.5 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.7 | 6.5 | 0 | 0 | [run](https://argusic.com/run/fcb7a3b8-8bcf-4774-b8ab-f3300939fcd0) |
| 2 | pass with mocks | 85.33 | 35 | 12.9 | 3 | 2 | [run](https://argusic.com/run/c2150be4-4680-4f59-88d4-546dbae586b0) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Doc-test code fence '''no_run on same line as preceding text in 4 config.rs files (amzn-codewhisperer-client, amzn-codewhisperer-streaming-client, amzn-consolas-client, amzn-qdeveloper-streaming-client)`
- 2 min: `Doc-test in chat-cli-ui/src/conduit.rs missing import for get_legacy_conduits`
- `3 doc-test failures in semantic-search-client (async_implementation.rs) not fixed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
