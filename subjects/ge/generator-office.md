# generator-office

**Verdict: runs.** Argusic Score 72.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OfficeDev/generator-office, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/generator-office

## Pinned environment

- Project commit: `106a1cf50c2ed009dc56cef5fb1e09e03e15c377`
- Test commit: `106a1cf50c2ed009dc56cef5fb1e09e03e15c377`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 52.3 to 84.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 45 | 52.3 | 9 | 9 | [run](https://argusic.com/run/02e2fe81-714b-4e1b-ba28-faeaa69a5074) |
| 2 | pass | 95 | 12 | 84.5 | 4 | 3 | [run](https://argusic.com/run/8db969d5-0a59-495a-9d21-b81ca16f1bbf) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node v18.19.1 does not satisfy engine requirement >=20.12.0`
- 3 min: `Private Azure DevOps npm registry in .npmrc blocks install with E401`
- 2 min: `mocha@12 and env-cmd@11 use import assertions syntax (with {type:'json'}) unsupported in Node 18`
- 10 min: `mem-fs-editor@12.1 uses /v regex flag (ES2024/Node 20+) in 9 dist files`
- 8 min: `yeoman-test@11.8.2 uses styleText from node:util (Node 20+), and @yeoman/conflicter uses similar Node 20 features`
- 5 min: `office-addin-manifest requires uuid@14 (ESM-only) but its own code uses require(), failing on Node 18`
- 3 min: `@microsoft/app-manifest requires strip-bom@5 (ESM) via CJS require()`
- 10 min: `Tests hang on GitHub template downloads via axios (network requests timeout)`
- 3 min: `TypeScript compilation errors when yeoman-generator is downgraded (v5 vs v7 types mismatch)`

Attempt 2:

- 4 min: `System Node is v18 but the repo requires >=20.12; npm install unsupported-engine and build steps fail`
- 5 min: `npm install failed E401/E404 because repo .npmrc and bundled package-lock.json pointed to a private Azure feed (office.pkgs.visualstudio.com)`
- 2 min: `First npm test run had 1 failure in the proxy-config test; the npx/mocha subprocess hit the private feed`
- 1 min: `Generated project's npm start fails because CA-cert install needs sudo (unavailable) and Office sideload is unsupported on linux; not fixable in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
