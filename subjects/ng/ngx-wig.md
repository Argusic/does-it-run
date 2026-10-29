# ngx-wig

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bampakoa/ngx-wig, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ngx-wig

## Pinned environment

- Project commit: `14588d09341b14cc9079b07df090d9b08407ecf9`
- Test commit: `14588d09341b14cc9079b07df090d9b08407ecf9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.7 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 8 | 7.7 | 4 | 3 | [run](https://argusic.com/run/354082b2-c828-4d7f-8967-9c6d8f49d006) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Bundled Node v18.19.1 too old for Angular 22 (CLI requires v22.22.3+)`
- 2 min: `No Chrome/Chromium binary in container; karma failed with 'No binary for ChromeHeadless'`
- 2 min: `ChromeHeadless failed with 'No usable sandbox' (unprivileged user namespaces disabled)`
- 1 min: `ng test ngx-wig-app fails: missing src/tsconfig.spec.json, src/test.ts, src/karma.conf.js referenced by angular.json app test target`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
