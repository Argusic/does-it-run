# Textus

**Verdict: runs.** Argusic Score 58 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CatVinci-Studio/Textus, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/textus

## Pinned environment

- Project commit: `6786182e72dca39e974a4128195835b7fa9aa70c`
- Test commit: `6786182e72dca39e974a4128195835b7fa9aa70c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 17.8 to 74.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 16 | 6 | 74.3 | 10 | 8 | [run](https://argusic.com/run/c70a61d7-f487-47c5-97cd-d20cc7db2a57) |
| 2 | pass | 100 | 1.5 | 17.8 | 6 | 6 | [run](https://argusic.com/run/4cce8383-9d54-48da-bd99-49fb842847a0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node 18.19.1 was installed, but package.json requires Node >=22.`
- 2 min: `Rust and Cargo were not installed; src-tauri/rust-toolchain.toml requires rustup.`
- 3 min: `The first full npm test run had scripts/release-notes.test.mjs time out at 5 seconds while the frontend build ran concurrently: 3388 passed, 1 failed.`
- 4 min: `npm run tauri build -- --debug failed: pkg-config could not find glib-2.0; WebKitGTK 4.1 development files were also absent.`
- 2 min: `The release AppImage could not mount because the container has no FUSE.`
- 3 min: `Initial e2e run failed market.spec.ts and native-web-page.spec.ts because the companion textus-plugins checkout was absent.`
- 3 min: `Seven chart e2e tests failed because the companion checkout's node_modules lacked chart libraries such as echarts.`
- 5 min: `The CJK table-header wrap e2e test failed because the container had zero Chinese fonts.`
- 10 min: `phone-quickask.spec.ts still fails in isolation: native Home stops at the start of the wrapped final visual line, so only 'months.' is selected instead of the whole paragraph.`
- 15 min: `database.spec.ts new-page creation failed with textus-plugins 0.4.0 because that version defines two addRow functions; the second overrides the table handler.`

Attempt 2:

- 4 min: `Container shipped Node v18.19.1, but the project requires Node >=22; npm install emitted dozens of EBADENGINE warnings and installed under the wrong runtime.`
- 1 min: `DENIED: I attempted to delete temporary file /work/repo/vite.verify-no-watch.config.mjs, but the environment rejected my file deletion request.`
- 6 min: `npm run setup:e2e initially could not start Vite: EMFILE: too many open files, watch '/work/repo/vite.katex-fonts.ts' (repeated twice, including on a fresh port).`
- 3 min: `The published Linux tarball binary exited 127 before startup: libwebkit2gtk-4.1.so.0: cannot open shared object file.`
- 3 min: `The production frontend served from 'vite preview' in a plain browser showed 'Something went wrong' with Cannot read properties of undefined (reading 'metadata'), because the Tauri IPC backend was absent.`
- 4 min: `npm run check:native failed compiling glib-sys: Package glib-2.0 was not found in the pkg-config search path.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
