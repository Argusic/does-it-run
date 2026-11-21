# free4chat

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/i365dev/free4chat, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/free4chat

## Pinned environment

- Project commit: `4dbf2e5b4f7bfdcbf71e152b037412e82fc0f53c`
- Test commit: `4dbf2e5b4f7bfdcbf71e152b037412e82fc0f53c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.3 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.3 | 1 | 1 | [run](https://argusic.com/run/8749b6a0-c4a9-4db2-8693-296b093210e7) |
| 2 | pass | 100 | 27 | 13.6 | 7 | 7 | [run](https://argusic.com/run/9c586f26-791b-4244-93d2-914646281f06) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go toolchain not found in container (requires Go 1.27+)`

Attempt 2:

- 2 min: `System Node.js 18.19.1 is too old (project requires >=20)`
- 1 min: `yarn not found on PATH`
- 2 min: `Go 1.23.0 download was a stale binary; go.mod requires go 1.27`
- 1 min: `yarn install failed: engine incompatibility with @modelcontextprotocol/server@2.0.0 (node >=20)`
- 3 min: `vitest runtimeProviderCredential tests failed: jsdom cross-realm WebCrypto TypeError on ArrayBuffer digest argument`
- 1 min: `opennextjs-cloudflare build rejected Next.js 15.5.24 as unsupported major`
- 1 min: `TypeScript tsc --noEmit failed after fix: Uint8Array<ArrayBufferLike> not assignable to BufferSource`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
