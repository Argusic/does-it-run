# design-studio

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Tiledesk/design-studio, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/design-studio

## Pinned environment

- Project commit: `b72ebaa8c73aa000741daf4d91378eb8bd2dfa7b`
- Test commit: `b72ebaa8c73aa000741daf4d91378eb8bd2dfa7b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28.5 to 28.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 28.5 | 6 | 6 | [run](https://argusic.com/run/8db85615-9792-4c0d-b3f9-ce84d83bfe8b) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Broken spec files with wrong component class names (17 files): toogle, advanced, cds-action-speech-form, cds-action-reply-button, cds-action-reply-voice-text, attributes-dialog, operand/operation/operator (v2), cds-action-email, cds-action-`
- 2 min: `Missing @ionic/angular module in user-typing.component.spec.ts`
- 1 min: `app.component.spec.ts tested non-existent title property`
- 5 min: `No Chrome browser installed in the container`
- `191 of 334 unit tests fail at runtime due to missing provider/pipe/module mocks in spec files (pre-existing test quality issues)`
- 1 min: `test.ts lacked require.context for spec discovery`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
