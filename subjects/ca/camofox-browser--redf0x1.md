# camofox-browser

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/redf0x1/camofox-browser, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/0218a48e-ba2b-41da-bf2b-c4f39025fec8

## Pinned environment

- Project commit: `4f23dcf30dc0a1fb20b1a94fd6035a000a31a8bd`
- Test commit: `4f23dcf30dc0a1fb20b1a94fd6035a000a31a8bd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 34.4 to 34.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 34.4 | 3 | 3 | [run](https://argusic.com/run/0218a48e-ba2b-41da-bf2b-c4f39025fec8) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18 installed but project requires >=20`
- 2 min: `npm install ran under Node 18, adding engine warnings and failing postinstall`
- 2 min: `better-sqlite3 native addon compiled against Node 18 ABI, segfaulting under Node 20 (SIGSEGV during WebGL sampling)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
