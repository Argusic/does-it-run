# excalidraw

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/excalidraw/excalidraw, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/excalidraw

## Pinned environment

- Project commit: `e1bb9ff8f8931e783c11d104abb8967ac6605c9a`
- Test commit: `e1bb9ff8f8931e783c11d104abb8967ac6605c9a`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 6; wall time 5.6 to 33.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 22.4 | 4 | 4 | [run](https://argusic.com/run/663ee5f3-d834-4bc2-9283-a853fb00523b) |
| 1 | pass | 100 | 0.5 | 24.3 | 1 | 1 | [run](https://argusic.com/run/624cff53-04eb-4844-aac7-c984010ae599) |
| 2 | pass | 100 | 3.5 | 17.6 | 3 | 3 | [run](https://argusic.com/run/8e319e6b-462a-4bb7-aa72-1f5ab39414bb) |
| 2 | pass | 100 | 0.2 | 5.6 | 2 | 2 | [run](https://argusic.com/run/829ca649-59cc-42a5-967f-c3a4d00e4af6) |
| 3 | pass | 100 | 2 | 13.8 | 5 | 5 | [run](https://argusic.com/run/3392e83b-d79b-4efc-a22a-d805e8126214) |
| 3 | pass | 100 | 3 | 33.5 | 2 | 2 | [run](https://argusic.com/run/e477c9df-3639-4a3f-b4dd-2bdc4d3b2887) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `yarn: command not found , dev docs and package.json packageManager require Yarn 1.22.22, container had neither yarn nor corepack`
- 1 min: `npm install -g failed with EACCES writing to /usr/local prefix; no root and no sudo in container`
- 4 min: `yarn install aborted: 'error marked@16.4.2: The engine node is incompatible with this module. Expected version >= 20. Got 18.19.1' (transitive via @excalidraw/mermaid-to-excalidraw -> mermaid), despite engines.node declaring >=18.0.0`
- 4 min: `Playwright Chromium refused to launch: 13 missing system shared libs (libnss3, libatk, libasound, libxkbcommon, ...), no root for apt-get install`

Attempt 1:

- 3 min: `3 failing tests in animation.test.ts due to vitest 3.x jsdom environment baseline timer and recursive runOnlyPendingTimersAsync behavior`

Attempt 2:

- 1 min: `yarn not installed; npm i -g yarn failed with EACCES on /usr/local/lib/node_modules, and 'npm config set prefix' wrote prefix= into the repo's own .npmrc (project scope, ignored by -g)`
- 2 min: `yarn install aborted: error marked@16.4.2: The engine "node" is incompatible with this module. Expected version ">= 20". Got "18.19.1" (marked hoisted from @excalidraw/excalidraw > @excalidraw/mermaid-to-excalidraw > mermaid); root package.`
- 3 min: `Headless Chromium refused to launch: 'Host system is missing dependencies to run browsers' (libnss3, libnspr4, libatk1.0-0t64, libatk-bridge2.0-0t64, libatspi2.0-0t64, libxdamage1, libxkbcommon0, libasound2t64); no root or sudo available`

Attempt 2:

- 0.1 min: `Global yarn not installed; used npx yarn instead`
- 0.1 min: `marked@16.4.2 requires node >=20, but node 18.19.1 is installed`

Attempt 3:

- 2 min: `yarn (required package manager, pinned 1.22.22) not installed; 'npm install -g yarn' failed with EACCES: permission denied, mkdir '/usr/local/lib/node_modules/yarn' (no root in container)`
- 1 min: `'yarn install --frozen-lockfile' aborted: 'error marked@16.4.2: The engine "node" is incompatible with this module. Expected version ">= 20". Got "18.19.1"'`
- 1 min: `'yarn start' re-triggers the marked engine error, because excalidraw-app's start script is 'yarn && vite' and the nested install re-runs the engine check`
- 1 min: `'npx @puppeteer/browsers install chrome@stable' (for browser verification) crashed on Node 18: 'SyntaxError: Invalid regular expression flags' , latest version uses the ES2024 regex 'v' flag requiring Node 20+`
- 3 min: `Downloaded Chrome failed to launch: 'error while loading shared libraries: libnss3.so: cannot open shared object file'; ldd showed ~20 missing libs (nss, nspr, atk, cairo, pango, cups, asound, xkbcommon, harfbuzz, avahi, ...) and there is n`

Attempt 3:

- 2 min: `Test 'frame + labeled arrow' in actionDeleteSelected.test.tsx fails with 'still loading' timeout when running full suite`
- 2 min: `Test 'should eventually initialize all images added through image tool' in history.test.tsx fails with empty elements when running full suite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
