# drawio-skill

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Agents365-ai/drawio-skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/drawio-skill

## Pinned environment

- Project commit: `7b996a17d05509bac95227c8e58397a8a175a1b9`
- Test commit: `7b996a17d05509bac95227c8e58397a8a175a1b9`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 5.8 to 14.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 14.6 | 1 | 1 | [run](https://argusic.com/run/15bdc678-5096-403c-9351-2d932050de25) |
| 2 | pass | 100 | 0 | 10.3 | 1 | 1 | [run](https://argusic.com/run/7718f1ab-4997-47ea-9086-156d54cd1ca2) |
| 3 | pass with mocks | 92 | 0 | 5.8 | 1 | 1 | [run](https://argusic.com/run/c5f1dc60-33c2-4cba-8277-046d41e8cd88) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_views_and_story_are_accessible failed: _grid_page fallback (when Graphviz dot is absent) did not emit UserObject wrappers for page-link navigation`

Attempt 2:

- 3 min: `test_views_and_story_are_accessible failed: write_drawio fallback (_grid_page) did not emit UserObject wrappers for cross-page linked nodes when Graphviz was absent`

Attempt 3:

- 2 min: `test_views_and_story_are_accessible failed because _grid_page (fallback when Graphviz dot not available) did not wrap linked nodes in UserObject elements`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
