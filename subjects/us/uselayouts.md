# uselayouts

**Verdict: runs.** Argusic Score 87.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iurvish/uselayouts, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/uselayouts

## Pinned environment

- Project commit: `5ed0d94454374b47ed9805bf204a412bc2d3d456`
- Test commit: `5ed0d94454374b47ed9805bf204a412bc2d3d456`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 4; wall time 12.6 to 62.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 14.8 | 3 | 3 | [run](https://argusic.com/run/2d1bfdff-5568-4d6c-a386-23a52db15a5c) |
| 1 | pass | 100 | 12.4 | 12.6 | 3 | 3 | [run](https://argusic.com/run/7aa90c4e-a781-4b47-bafa-b8cb0bcc911f) |
| 2 | pass | 100 | 25 | 24.2 | 3 | 3 | [run](https://argusic.com/run/2ec9317d-3a5e-4625-8a54-e6704dc0c04e) |
| 3 | fail | 50 | 2 | 62.1 | 8 | 8 | [run](https://argusic.com/run/97e4a628-05ae-45a8-8c4d-ae0063ceafa8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18.19.1 is too old for Next.js 16 (requires >=20.9.0)`
- 1 min: `build-registry.mts uses 'bun x shadcn' but bun is not available`
- 2 min: `Tailwind CSS v4 cannot apply unknown utility class '-inset-s-4' in fumadocs-ui/css/lib/base.css`

Attempt 1:

- 3 min: `Node.js v18.19.1 is too old for Next.js 16 which requires >=20.9.0`
- 1 min: `build-registry.mts script uses 'bun x shadcn' but bun is not installed`
- 2 min: `Tailwind CSS v4 rejects '-inset-s-4' in @apply because negative logical-property utilities are unsupported in Tailwind v4`

Attempt 2:

- 2 min: `build-registry.mts uses 'bun x shadcn' but bun is not available`
- 3 min: `Next.js 16 requires Node >=20.9.0, container has Node 18`
- 15 min: `Tailwind v4 does not recognize fumadocs-ui's 'inset-s-*' and 'inset-e-*' utility classes`

Attempt 3:

- 1 min: `bun not installed , build-registry script used bun x shadcn`
- 5 min: `fumadocs-mdx:collections/server virtual module scheme not handled by webpack (UnhandledSchemeError)`
- 10 min: `Next.js 16 requires Node >=20.9.0, container has Node 18.19.1`
- 5 min: `Tailwind CSS v4.1.18 cannot apply unknown utility class '-inset-s-4'`
- 20 min: `useEffectEvent not exported from react in Next.js 15.3.2's compiled React (19.2.0-canary)`
- 3 min: `ESLint config module resolution fails in flat config format`
- 1 min: `React 19.2.8/react-dom 19.2.3 version mismatch`
- 10 min: `Next.js build OOM during static page generation (772MB total memory, 35 pages)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
