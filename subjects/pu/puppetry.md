# puppetry

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dsheiko/puppetry, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/puppetry

## Pinned environment

- Project commit: `d0fdb94cd44621a91aeb9c689b9b8463061792cd`
- Test commit: `d0fdb94cd44621a91aeb9c689b9b8463061792cd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.9 to 21.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 14.9 | 2 | 2 | [run](https://argusic.com/run/b4f8eaa5-b998-4328-81bb-ca75e6a5751d) |
| 2 | pass | 100 | 4 | 21.1 | 2 | 2 | [run](https://argusic.com/run/d9a8439d-226a-43a2-baec-15fbeafb3a86) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `jest tests fail with Cannot find module 'node:stream' from cheerio 1.2.0 (ESM-only, node: protocol not supported by jest 24)`
- 2 min: `electron binary fails with SUID sandbox helper not configured correctly (no root in container)`

Attempt 2:

- 1 min: `Jest 24 resolver does not support the node: protocol prefix (e.g. require('node:stream')) used by modern dependencies like parse5-parser-stream, encoding-sniffer, htmlparser2, minipass, undici`
- 2 min: `cheerio@1.2.0 (pulled by enzyme) depends on undici which references browser globals (ReadableStream, Blob, performance, Event, TextDecoder) not available in Jest 24 node environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
