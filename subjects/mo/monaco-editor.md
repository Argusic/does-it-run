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
- Valid runs: 1; wall time 17.8 to 17.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10.5 | 17.8 | 5 | 5 | [run](https://argusic.com/run/f756eb61-6034-4710-b2a5-5297a99c1f66) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `import.meta.dirname requires Node 22+ but container has Node 18.19.1; 5 build config files used it`
- 2 min: `jsdom v29 depends on @exodus/bytes (ESM-only package) which crashes require() on Node 18`
- 1 min: `crypto global not defined in test setup; monaco-editor-core calls crypto.randomUUID`
- 2 min: `AMD Vite build requires Node 20+; Vite 7 fails on Node 18`
- 0.5 min: `test:grammars script had quoted glob pattern that shell doesn't expand on Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
