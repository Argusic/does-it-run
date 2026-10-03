# nest

**Verdict: runs.** Argusic Score 86.4 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nestjs/nest, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nest

## Pinned environment

- Project commit: `1eeccd30a4cd23db5c1eb5539d49ff3fae4f2de6`
- Test commit: `1eeccd30a4cd23db5c1eb5539d49ff3fae4f2de6`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services, no run possible
- Valid runs: 6; wall time 5.4 to 59.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 5.4 | 3 | 3 | [run](https://argusic.com/run/4d06304d-d94a-4ac0-968a-b653bd3a5de7) |
| 1 | pass | 100 | 34 | 43.7 | 8 | 8 | [run](https://argusic.com/run/52d91431-3e3c-4130-bcef-d58aeda8b7f7) |
| 2 | pass with mocks | 82 | 5 | 12.8 | 2 | 1 | [run](https://argusic.com/run/f2cee4f8-647e-4d77-a651-fd05aaaf7e4c) |
| 2 | pass | 100 | 15 | 14.7 | 3 | 3 | [run](https://argusic.com/run/d39c014f-fde0-4e7a-82c2-1839e12cc2b5) |
| 3 | fail | 36.67 | 5 | 14.5 | 3 | 1 | [run](https://argusic.com/run/fd666c30-7ea3-422a-9269-98550c4160f2) |
| 3 | pass | 100 | 2 | 59.9 | 4 | 4 | [run](https://argusic.com/run/bb82de0b-5dfb-4749-8dbf-61ae13dc2b03) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Peer dependency conflict: graphql version mismatch between @apollo/server and @nestjs/apollo`
- 2 min: `Node 18 lacks Node 20+ APIs: styleText and parseEnv from node:util`
- 1 min: `Missing rolldown native bindings for Linux x64`

Attempt 1:

- 1 min: `npm install failed: GraphQL peer dependency conflict`
- 3 min: `vitest 4.x requires rolldown, which needs Node 22 (container has Node 18)`
- 8 min: `Decorator metadata ('design:paramtypes') not emitted by esbuild (Node 18)`
- 5 min: `TypeScript paths (e.g. @nestjs/common/internal) not resolved by vitest`
- 10 min: `file-type v22 uses /v regex flag unsupported by Node 18`
- 3 min: `JSON.parse error message differs between Node 18 ('Unexpected end of JSON input') and Node 20+`
- 2 min: `Logger test expected ANSI color codes in util.inspect output not present in Node 18`
- 2 min: `Deep-hashed module opaque key test: function toString() representation differs across Node versions with oxc transform`

Attempt 2:

- `Node version 18.19.1 is below required 20+ - prevents running vitest and sample apps`
- 1 min: `npm ERESOLVE peer dependency conflict between graphql and @apollo/server versions`

Attempt 2:

- 2 min: `Peer dependency conflict: @apollo/server@5.5.1 requires graphql@^16.11.0 but graphql@17.0.2 is installed`
- 4 min: `vitest 4.x imports styleText from node:util which is unavailable in Node 18`
- 1 min: `1 test fails when NO_COLOR=1 env set (test expects ANSI codes, ConsoleLogger respects NO_COLOR)`

Attempt 3:

- 2 min: `graphql peer dependency conflict between @apollo/server@5.5.1 and graphql@17.0.2`
- 1 min: `vitest requires Node 20+ (util.styleText export missing in Node 18.19.1)`
- 1 min: `sample apps require Node 20+ (JSON import syntax not supported in Node 18.19.1)`

Attempt 3:

- 1 min: `Node.js v18 lacks 'styleText' in 'node:util' required by Vitest 4.x`
- 1 min: `npm peer dependency conflict: graphql@17.0.2 vs @apollo/server@5.5.1 expecting graphql@^16.11.0`
- `Integration test failures: SSE express (13) and durable-providers (2) fail due to disabled IPv6 loopback (::1) in container causing EADDRNOTAVAIL`
- `14 integration tests skip because MQTT/Kafka/Redis/RabbitMQ/NATS servers are unreachable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
