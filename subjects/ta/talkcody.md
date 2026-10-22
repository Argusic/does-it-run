# talkcody

**Verdict: runs with mocks.** Argusic Score 87 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/talkcody/talkcody, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/talkcody

## Pinned environment

- Project commit: `5543bf9264366daa2f26880095fc34e016ffb304`
- Test commit: `5543bf9264366daa2f26880095fc34e016ffb304`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 24.3 to 24.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 25 | 24.3 | 4 | 3 | [run](https://argusic.com/run/043fdf66-2b27-4d68-8d75-a1eb6fff210b) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Bun not installed (also no unzip binary); Node 18 too old for jsdom 28 (@exodus/bytes ERR_REQUIRE_ESM); rustup lacking; all fixed by user-level installs`
- 10 min: `apps/api 'bun run test' always failed: run-tests.ts spawns 'bun run test <files>' recursively, then production URL equals test URL and safety check aborts`
- 12 min: `auth-google.test.ts 'should redirect to Google' failed (400): app.request(path,{env}) does not pass env into c.env in Hono 4.10.3`
- 5 min: `Tauri/Rust desktop build cannot compile: glib-2.0 and webkit2gtk-4.1 dev packages absent (only runtime .so, no .pc), no root to install system packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
