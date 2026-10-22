# markdown-site

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/waynesutton/markdown-site, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/markdown-site

## Pinned environment

- Project commit: `3872c59b58970144442091fc2a39f6b02846c582`
- Test commit: `3872c59b58970144442091fc2a39f6b02846c582`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 34.9 to 34.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 34.9 | 7 | 7 | [run](https://argusic.com/run/0670f08b-91de-4853-ae4d-3afefdd3f473) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing @robelest/samlify dependency (package unpublished from npm registry)`
- 2 min: `Node.js v18.19.1 too old for Vite 7.3.2 (requires 20.19+ or 22.12+)`
- 2 min: `createAuth renamed to defineAuth in convex-auth 0.0.4-preview.40`
- 3 min: `ComponentApi.public.userGetById and userList removed in new convex-auth`
- 1 min: `auth.http.add renamed to auth.request.mount`
- 2 min: `Auth client API changed: .state/.onChange replaced with getSnapshot()/subscribe()`
- `3 pre-existing TS errors in convex/files.ts (convex-fs@0.2.0 types incompat with convex@1.47.0)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
