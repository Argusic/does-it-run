# blender-ai-mcp-addon

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LiCinCan/blender-ai-mcp-addon, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/blender-ai-mcp-addon

## Pinned environment

- Project commit: `ce76f5c2623d264c8c8a2fe57b0830462555d61c`
- Test commit: `ce76f5c2623d264c8c8a2fe57b0830462555d61c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 84.2 to 84.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 48 | 84.2 | 5 | 5 | [run](https://argusic.com/run/fc3c0d1e-4897-4eb0-b613-9248d70f018a) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Blender not installed in container and addon requires Blender 4.2+ (system installs unavailable)`
- 8 min: `Background Blender exits right after its --python script and the mainthread queue never pumps; earlier MCP calls hung`
- 2 min: `Tool call move_object with argument delta was rejected (schema allows location/rotation/scale only) - not a bug, my call was wrong`
- 12 min: `Auth gate: with mcp_require_token=True, module _token stayed None in every launched run and no/wrong/right Bearer tokens all got HTTP 200; the Handler replica with _token set returns 401 as coded`
- 45 min: `HTTP MCP listener dies early on this container while Blender process stays alive (observed death windows 60s-3min; one 3min run stayed alive with listener already gone)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
