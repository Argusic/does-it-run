# ImGuiColorTextEdit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BalazsJako/ImGuiColorTextEdit, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/imguicolortextedit

## Pinned environment

- Project commit: `ca2f9f1462e3b60e56351bc466acda448c5ea50d`
- Test commit: `ca2f9f1462e3b60e56351bc466acda448c5ea50d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.2 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 10.2 | 1 | 1 | [run](https://argusic.com/run/00fd04ac-006e-4075-a5d6-dcdad522136c) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `TextEditor.cpp uses ImGui::PushItemFlag / ImGuiItemFlags_NoTabStop / ImGui::PopItemFlag from imgui_internal.h but only included imgui.h`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
