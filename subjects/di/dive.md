# Dive

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenAgentPlatform/Dive, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dive

## Pinned environment

- Project commit: `5fb62b91b55c4b781af71e43750574a2a1642416`
- Test commit: `5fb62b91b55c4b781af71e43750574a2a1642416`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 26.5 to 26.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 31 | 26.5 | 6 | 6 | [run](https://argusic.com/run/d66076a6-5295-494d-8006-34aeb382c4a1) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `npm install postinstall failed with TypeError on @electron/rebuild (node-gyp 'paths[0]' undefined) under system Node v18.19.1 (project's vite/vitest require ^20.19/22.x)`
- 8 min: `'npm run dev' and 'npx vite --config vite.config.electron.ts' in dev mode fataled on 'SUID sandbox helper ... not configured correctly' (container chrome-sandbox lacks root:root 4755)`
- 3 min: `Electron dev-mode renderer invoked 'util:setModelSettings' but config dir did not exist, causing repeated Unhandled Rejection ENOENT .config/model_settings.json`
- 5 min: `mcp-host failed gradle-style at parser lock due to sandbox: 'uv' binary not in container; 'pip3 install uv' blocked by PEP 668 externally-managed environment, and README's 'uv sync' (mcp-host) is a required step`
- 2 min: `Electron standalone (without VITE_DEV_SERVER_URL) spawns 'uv run dive_httpd' from repo root where there is no pyproject.toml, so the host exited code 2 and the app reported no server`
- 1 min: `First Electron launch SIGILL-crashed renderer after the OAP plugin reached the real proxy.oaphub.ai (remote OAuth loop; CPU+crash); transient and occurred once, not reproducible`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
