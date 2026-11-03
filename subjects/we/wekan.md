# wekan

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wekan/wekan, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/wekan

## Pinned environment

- Project commit: `0e77fbb9d9b30673c26163a21889cdc95eb69511`
- Test commit: `0e77fbb9d9b30673c26163a21889cdc95eb69511`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 13.2 to 72.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 71 | 72.6 | 4 | 4 | [run](https://argusic.com/run/95a5c3ff-32c4-4a14-8f4f-ce8c2e151681) |
| 2 | pass | 80 | 5 | 13.2 | 15 | 0 | [run](https://argusic.com/run/fe8f7cfe-2a22-4093-a364-3aa6d1ce5305) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `system Node.js v18.19.1 is too old (project requires 26.x); npm 9 cannot parse the npm: alias syntax in package.json overrides`
- 5 min: `MongoDB not pre-installed in the container`
- `129 of 1226 plain-Node test suites failed (10.5%) , mostly translation placeholder-audit failures due to changed Meteor/npm version strings, git-history-dependent changelog tests, and missing MongoDB/Meteor runtime for integration tests`
- 2 min: `package.json sourcemap-codec override uses npm: alias syntax unsupported by npm 9 but required for Rspack compat`

Attempt 2:

- `Translation-progress tests (70+) fail because the test expects specific translation stats that don't match current repo state`
- `changelogFormat.test.cjs: 20 over-long lines without links in CHANGELOG.md`
- `changelogHashFix.test.cjs: related to changelog format issues`
- `docsLinksResolve.test.cjs: 4 docs links to models/eventlog.js don't resolve`
- `oidcProfileMerge.test.cjs: adminCreation is not defined in extracted server/models/users.js`
- `restLdapLogin.test.cjs: expects Accounts._insertLoginToken pattern not found in source`
- `restSecurityAdvisories.test.cjs: expects audit record before impersonation token`
- `activeForgeMirror.test.cjs: expects hardcoded git mirror path`
- `adminPanelDocsMatchMenu.test.cjs: expects auth docs sections that differ`
- `fontAwesomeIcons.test.cjs: unicode arrows where fa icons expected`
- `fossilExport.test.cjs: needs 'fossil' binary not in container`
- `listBodyDragLifecycle.test.cjs: pre-existing test concept mismatch`
- `popupTitles.test.cjs: expects no moveObjects titles`
- `uiFonts.test.cjs: UI-related test incompatible with headless`
- `e2eSessionTokens.test.cjs: needs running full server stack`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
