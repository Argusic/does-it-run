# web-maker

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chinchang/web-maker, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/web-maker

## Pinned environment

- Project commit: `b1cb6071eb99f28078f732b8bec3dfb47af5c241`
- Test commit: `b1cb6071eb99f28078f732b8bec3dfb47af5c241`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 20.1 to 20.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 19 | 20.1 | 6 | 6 | [run](https://argusic.com/run/b72267ed-f5f9-4f89-8278-95724a230372) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Cannot find module preact-cli/babel - preact-cli@4.0.0-next.6 npm package is missing its babel/ directory`
- 2 min: `.babelrc circular config load caused Babel validation error in Jest`
- 1 min: `Cypress tests picked up by Jest due to missing testPathIgnorePatterns entry`
- 2 min: `Cannot find module preact-render-spy for fileUtils.test.js`
- 5 min: `layout-parameter.test.js failures from jsdom location.search navigation side effects`
- 4 min: `Can't resolve monaco-editor/esm/vs/editor/editor.api.js - y-monaco cannot resolve due to monaco-editor@0.57.0 exports map`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
