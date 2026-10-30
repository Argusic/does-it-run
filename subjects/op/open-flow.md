# open-flow

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/oomol-lab/open-flow, licensed NOASSERTION, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/open-flow

## Pinned environment

- Project commit: `29c74de02e6d9e597633fecb6ece0d7f36806f27`
- Test commit: `29c74de02e6d9e597633fecb6ece0d7f36806f27`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.6 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 9 | 13.6 | 4 | 3 | [run](https://argusic.com/run/cfb9d43b-6080-4d94-9b9b-236c52466e4a) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `Bun not installed in base container`
- 0.7 min: `Node 18.19.1 in base container, project requires Node 26`
- 1 min: `bun install --frozen-lockfile failed: isolated-vm compiled against Node 18 headers and failed with C++ errors`
- `test/mcp.test.ts: 'enforces authentication, Origin, request limits and the modern HTTP protocol' consistently fails with SocketError: other side closed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
