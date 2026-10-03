# upstat

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chamanbravo/upstat, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/upstat

## Pinned environment

- Project commit: `658b6d29e4c6621a437b20d1cc54143dbe6f8bf5`
- Test commit: `658b6d29e4c6621a437b20d1cc54143dbe6f8bf5`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 16.9 to 37.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 37.4 | 3 | 3 | [run](https://argusic.com/run/1e4aa89b-77d8-4d71-848f-c050ba2f9b5a) |
| 2 | pass | 100 | 16 | 16.9 | 3 | 3 | [run](https://argusic.com/run/b818ba70-6353-4d8d-8a71-b270a0edc3ac) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go compiler not installed in container`
- 8 min: `CGO required for go-sqlite3 but gcc not available`
- 5 min: `Auto-generated TypeScript types have id?: string instead of id?: number for API monitor schemas`

Attempt 2:

- 3 min: `Go is not installed in the container`
- 0.5 min: `.env default (DB_TYPE=postgres) causes panic , no Postgres server available`
- 3 min: `Generated TypeScript types declare MonitorItem.id as optional string (id?: string) but the component expects id: number`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
