# monaco-editor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/monaco-editor, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/monaco-editor

## Pinned environment

- Project commit: `fdf1ee75a63b85433a591db4e1184022cad8483b`
- Test commit: `fdf1ee75a63b85433a591db4e1184022cad8483b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 11.1 to 17.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10.5 | 17.8 | 5 | 5 | [run](https://argusic.com/run/f756eb61-6034-4710-b2a5-5297a99c1f66) |
| 2 | pass | 100 | 17 | 11.1 | 5 | 5 | [run](https://argusic.com/run/bf416c13-8a51-4ef4-9caf-1e94d18e0f94) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `import.meta.dirname requires Node 22+ but container has Node 18.19.1; 5 build config files used it`
- 2 min: `jsdom v29 depends on @exodus/bytes (ESM-only package) which crashes require() on Node 18`
- 1 min: `crypto global not defined in test setup; monaco-editor-core calls crypto.randomUUID`
- 2 min: `AMD Vite build requires Node 20+; Vite 7 fails on Node 18`
- 0.5 min: `test:grammars script had quoted glob pattern that shell doesn't expand on Node 18`

Attempt 2:

- 3 min: `import.meta.dirname is Node.js 20+ feature; 4 config files + 1 lsp client config fail on Node 18`
- 2 min: `jsdom@29.0.1 depends on html-encoding-sniffer which requires Node 20+; crashes test suite with ERR_REQUIRE_ESM`
- 2 min: `Missing globalThis.crypto in JSDOM environment , monaco-editor-core uses crypto.randomUUID at import time`
- 1 min: `npm test fails because test:grammars script in package.json has glob pattern in quotes preventing shell expansion`
- 1 min: `@rolldown/binding-linux-x64-gnu optional dependency not installed for monaco-lsp-client rolldown build`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
