# graphql-cli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Urigo/graphql-cli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/graphql-cli

## Pinned environment

- Project commit: `aa709566b74a3ee177c54f7dca909c1c4f75a598`
- Test commit: `aa709566b74a3ee177c54f7dca909c1c4f75a598`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15 to 15 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 15 | 4 | 4 | [run](https://argusic.com/run/c265282d-8b6d-4d1d-a328-2d11990d4f26) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `yarn not in PATH while lerna.json configured for yarn`
- 4 min: `UrlLoader type mismatch: DocumentLoader.load() returns Promise<Source> but Loader expects Promise<Source[]>`
- 7 min: `@graphql-cli/common type error: root @graphql-tools/utils v8 Loader incompatible with @graphql-tools/load's nested v7 loader types`
- 2 min: `website build failed: ERR_OSSL_EVP_UNSUPPORTED on Node 18 with webpack`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
