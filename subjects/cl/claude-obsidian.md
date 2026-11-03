# claude-obsidian

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AgriciDaniel/claude-obsidian, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-obsidian

## Pinned environment

- Project commit: `ad67087cad22ad84cc3288f915588ae42c0c2b44`
- Test commit: `ad67087cad22ad84cc3288f915588ae42c0c2b44`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.7 to 5.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.25 | 5.5 | 0 | 0 | [run](https://argusic.com/run/bff32db0-acb7-4919-af90-84b8090a02fd) |
| 2 | pass | 100 | 5 | 4.7 | 4 | 4 | [run](https://argusic.com/run/69fa1056-dee8-4a43-b855-b5319a6ad41c) |

## What was observed on a clean machine

Attempt 2:

- `A fresh-vault setup command was rejected by the command guard because it began with rm -rf.`
- `capture adapters --vault PATH exited with argparse error: unrecognized arguments.`
- `Assumed setup-retrieve.sh preview output was JSON, causing JSONDecodeError.`
- 1 min: `First test fixture used [[Cobalt Lantern]] while the file was Cobalt-Lantern.md, so strict lint reported 3 dead links and 1 orphan (5 issues).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
