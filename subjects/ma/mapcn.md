# mapcn

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AnmolSaini16/mapcn, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mapcn

## Pinned environment

- Project commit: `d160bd767bc6388618720c6038a4dd9948c97362`
- Test commit: `d160bd767bc6388618720c6038a4dd9948c97362`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 4.4 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 8.1 | 2 | 2 | [run](https://argusic.com/run/054bb1c4-9faa-45fe-a7d1-4a00fdd13a77) |
| 1 | pass | 100 | 3 | 4.4 | 1 | 1 | [run](https://argusic.com/run/d13a9fe8-40bd-4dd5-9b75-e39f74eb6df9) |
| 2 | pass | 100 | 9.1 | 5.8 | 3 | 3 | [run](https://argusic.com/run/09d27f47-3efe-43e1-b5e9-a0a46b01ed07) |
| 3 | pass | 100 | 5 | 6 | 1 | 1 | [run](https://argusic.com/run/703f7cfa-4314-4685-ad57-891335fe8d61) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18.19.1 is too old , Next.js 16 requires >=20.9.0. npm install succeeded with warnings, but 'next build' failed immediately with a version error.`
- 1 min: `Lint error in src/components/ui/sidebar.tsx:611 , 'Math.random' called during render in skeleton width calculation, triggering react-hooks/purity rule.`

Attempt 1:

- 2 min: `Node.js v18.19.1 is too old for Next.js 16 (requires >=20.9.0), causing build to abort`

Attempt 2:

- 2.5 min: `Node.js v18.19.1 is too old for Next.js 16 (requires >=20.9.0). Build fails immediately with 'Node.js version >=20.9.0 is required'.`
- 1.5 min: `Build fails with ESLint error: 'Math.random' is an impure function in src/components/ui/sidebar.tsx:611 inside React.useMemo`
- 0.5 min: `Build warning: unused import 'DocsLink' in src/app/(main)/docs/routes/page.tsx:5`

Attempt 3:

- 2 min: `Node.js v18.19.1 is too old for Next.js 16 (requires >=20.9.0). npm install printed EBADENGINE warnings for several packages and next build failed with 'You are using Node.js 18.19.1. For Next.js, Node.js version >=20.9.0 is required.'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
