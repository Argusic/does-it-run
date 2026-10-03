# hot-updater

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gronxb/hot-updater, licensed NOASSERTION, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hot-updater

## Pinned environment

- Project commit: `35964bb6cf0252f6385e29dcd0b3023744cb31a4`
- Test commit: `35964bb6cf0252f6385e29dcd0b3023744cb31a4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 12.9 to 35.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 31 | 35.3 | 4 | 4 | [run](https://argusic.com/run/64f4b23b-fbbe-42c0-ae70-1ef9da5dec26) |
| 1 | pass | 80 | 1.8 | 16.7 | 2 | 0 | [run](https://argusic.com/run/47f683b6-9529-45e9-9499-dde455d35f93) |
| 2 | pass | 100 | 2 | 12.9 | 2 | 2 | [run](https://argusic.com/run/72b0fb2c-d40e-416c-b78c-818614c4d3fb) |
| 3 | pass | 100 | 15 | 16.6 | 2 | 2 | [run](https://argusic.com/run/08bf8432-35e8-443d-a254-b7f807a02779) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js v18 is too old (needs >=22.13)`
- 1 min: `pnpm not available on PATH`
- 5 min: `Native Rust bindings for rolldown, oxc-parser, oxc-transform not installed (pnpm optional dep handling)`
- 3 min: `react-native-builder-bob (CJS) uses require() on ESM-only yargs 18; jsdom's html-encoding-sniffer requires ESM-only @exodus/bytes`

Attempt 1:

- 2 min: `Integration tests require Firebase emulator which needs Java (not installed in container)`
- `Integration tests also require Docker (for Supabase) and third-party cloud credentials (AWS, Cloudflare, Supabase)`

Attempt 2:

- 3 min: `pnpm not available with system Node 18; had to install pnpm via standalone installer and Node 22 via binary download`
- `Integration tests require Java (Firebase emulator) - not available in container`

Attempt 3:

- 3 min: `Node.js v18 lacked 'node:util.styleText' required by fumadocs-mdx postinstall script, causing docs postinstall to fail on first pnpm install attempt. Installed pnpm with npm -g (no root).`
- 6 min: `Test 'finds staged migrations when npx runs from the workspace root' failed because the mock used 'npx --no-install -- node probePath ...' which only works when 'node' is already in npx cache , not the case in this clean container.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
