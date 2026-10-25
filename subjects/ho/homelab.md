# homelab

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mortennordbye/homelab, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/homelab

## Pinned environment

- Project commit: `b30fa45d4568bfb2830811e3d43f0f32cb97d908`
- Test commit: `b30fa45d4568bfb2830811e3d43f0f32cb97d908`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.2 to 19.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 19.2 | 3 | 3 | [run](https://argusic.com/run/1af5024f-9597-4fd2-af0c-14b0cb843d4d) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Node.js 18.19.1 installed but Next.js 16 requires >=20.9.0; also @tailwindcss/oxide native .node module fails to resolve during Turbopack bundling because the bundled code uses relative require() for the NAPI binary but the binary lives in`
- 2 min: `Hugo not installed in container`
- 1 min: `TypeScript type-checker ran out of memory (2GB default heap)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
