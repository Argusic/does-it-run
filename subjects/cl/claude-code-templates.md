# claude-code-templates

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/davila7/claude-code-templates, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-code-templates

## Pinned environment

- Project commit: `5cc17cf267132cc690dee82239b80a99ec82e4f8`
- Test commit: `5cc17cf267132cc690dee82239b80a99ec82e4f8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 35.3 to 70.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.3 | 70.1 | 8 | 8 | [run](https://argusic.com/run/11ee6280-3460-4017-ae74-133109eeea43) |
| 2 | pass | 100 | 30 | 35.3 | 9 | 9 | [run](https://argusic.com/run/a9a13e01-17cb-4976-a985-e3e6b3d5ad67) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `@clack/prompts@1.7.0 ships ESM only (requires Node >=20.12), but the container has Node 18.19. The CLI fails at startup with ERR_REQUIRE_ESM.`
- 10 min: `StateService.test.js and DataService.test.js used 'const module = {exports:{}}; eval(sourceCXode)' which fails in Jest 30 because the test file's own 'module' binding shadows the local variable.`
- 2 min: `DataService.test.js failed to exit due to live setInterval from fallback polling started by the constructor.`
- 8 min: `WebSocketServer.test.js mocked ws.Server with 'jest.mock('ws')' but the mock had no return value for the close callback, causing close(client) to hang. getStats test used clients without ws property. global mock leak caused cross-test pollu`
- 12 min: `StateCalculator.determineConversationStatus returned different status labels ('active','inactive','recent') than tests expected ('waiting','idle','completed'). determineConversationState returned strings, not objects. quickStateCalculation`
- 12 min: `DataCache constructor referenced 'this.config.parsedDataTTL' before 'this.config' existed (self-reference). caches.parsedData and computationResults were missing but tests referenced them. getFileContent used stats.mtime.getTime() but fs mo`
- 2 min: `PerformanceMonitor test used setTimeout expectation pattern which failed because the test completed before the callback fired.`
- 3 min: `StateService.resetState called setState which sets lastUpdate=Date.now(), causing test failure. setError called setState which also set Error as a conversation, messing up history.`

Attempt 2:

- 8 min: `@clack/prompts v1.5.1 is ESM-only but Node 18 requires CJS require()`
- 3 min: `StateService.test.js and DataService.test.js used eval() with 'module' as a reserved variable name in Jest, causing SyntaxError`
- 3 min: `StateCalculator source has been refactored and no longer returns 'waiting','idle','completed' statuses, and isMissing isRecentActivity/getTimeSinceLastActivity methods`
- 4 min: `WebSocketServer.test.js failed because jest.mock('ws') auto-mock doesn't expose .Server as a constructor`
- 2 min: `PerformanceMonitor.test.js assumed methods (getCounter, resetCounters, generateReport) that don't exist`
- 2 min: `DataCache.test.js assumed different stats shape and that constructor accepts config arg`
- 2 min: `ReferenceValidator.test.js regex captures ')' in markdown URL causing plain URL extraction to match closing paren`
- 2 min: `IntegrityValidator output shape didn't include hashVerified field`
- 2 min: `Integration test used analytics module which has deeper dependencies`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
