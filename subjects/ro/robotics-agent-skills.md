# robotics-agent-skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/arpitg1304/robotics-agent-skills, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/robotics-agent-skills

## Pinned environment

- Project commit: `f9bc5467ff9ee3d23f1a1b0b29a649843bb6ad11`
- Test commit: `f9bc5467ff9ee3d23f1a1b0b29a649843bb6ad11`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9.8 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 35 | 9.8 | 3 | 3 | [run](https://argusic.com/run/9065543e-804d-4a75-9ccd-146bba6e1d90) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No pytest/numpy in environment; pip blocked by PEP 668 externally-managed environment`
- 18 min: `eval package imports failed: demo_recorder_node.py imported rclpy/rcl_interfaces/sensor_msgs at module level (no try/except), custom msg/srv modules missing because ROS2 IDL generation never ran without a ROS2 workspace`
- 6 min: `Episode JSON save raised TypeError: Object of type method is not JSON serializable; on_cleanup assumed buffers always exist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
