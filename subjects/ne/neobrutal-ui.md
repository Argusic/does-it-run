# neobrutal-ui

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Bridgetamana/neobrutal-ui, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/neobrutal-ui

## Pinned environment

- Project commit: `e0e95f8c82d5511aef47990f218f00425110fe89`
- Test commit: `e0e95f8c82d5511aef47990f218f00425110fe89`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 8.1 to 27.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 27.3 | 4 | 4 | [run](https://argusic.com/run/1e418527-c053-483a-9993-4116e05b971d) |
| 1 | pass | 100 | 9.5 | 21.9 | 3 | 3 | [run](https://argusic.com/run/f59458d0-74c7-4873-8f6a-497c5c12a211) |
| 2 | pass | 100 | 28 | 10.4 | 2 | 2 | [run](https://argusic.com/run/740966c2-76a6-4812-a1c0-4f63af477358) |
| 3 | pass | 100 | 3 | 8.1 | 1 | 1 | [run](https://argusic.com/run/96412c3f-a1c2-4b70-9653-b7dbdb7c3c5a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18.19.1 too old for Next.js 16 (requires >=20.9.0) , npm install succeeded but build immediately failed`
- 2 min: `Missing @tailwindcss/oxide-linux-x64-gnu native binding , first npm install with Node 18 didn't install optional native packages`
- `TypeScript build OOM during type checking with default memory`
- `TS2322: usePathname() returns string|null but SidebarContent expected string (2 occurrences)`

Attempt 1:

- 3 min: `Next.js 16 requires Node.js >=20.9.0, but container has Node.js 18.19.1`
- 1 min: `@tailwindcss/oxide native binding missing (npm optional dependency bug)`
- 1.5 min: `TypeScript 6 enforces noUncheckedSideEffectImports; import of './globals.css' has no type declarations`

Attempt 2:

- 3 min: `Node.js 18.19.1 is insufficient for Next.js 16 which requires Node >=20.9.0`
- 2 min: `npm install needed to be re-run after switching Node versions`

Attempt 3:

- 2 min: `System Node.js v18.19.1 is too old for Next.js v16.3.3 (requires >=20.9.0). The base npm install emitted 'unsupported engine' warnings but still completed, but next build refused to run.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
