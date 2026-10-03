# openagent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/the-open-agent/openagent, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/openagent

## Pinned environment

- Project commit: `45c53053eccf4d82f4e22a718ae87edc82fbff66`
- Test commit: `45c53053eccf4d82f4e22a718ae87edc82fbff66`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 38.8 to 42.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42.1 | 0 | 0 | [run](https://argusic.com/run/5461ed67-06bb-4528-bcc6-5cbb5a2fd460) |
| 2 | pass | 100 | 15 | 38.8 | 7 | 7 | [run](https://argusic.com/run/c4393128-6f1a-4da6-83ca-b916b24c9020) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `Go 1.25.0+ not installed`
- 3 min: `go build fails with 'non-constant format string in call to fmt.Errorf' in 234 places across ~70 files`
- 5 min: `App crashes at startup: 'exec: lsof: executable file not found in $PATH'`
- 1 min: `object/org_test.go and object/name_test.go reference nonexistent Chat.User1 and Chat.Users fields (now Chat.User)`
- 1 min: `object/video_import_test.go references undefined functions importVideos and importVideos2`
- 1 min: `model/gemini_test.go panics with empty API key`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
