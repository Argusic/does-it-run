# TensorFold

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ashhart/TensorFold, licensed Apache-2.0, written in Zig.

Evidence and recordings: https://argusic.com/subject/tensorfold

## Pinned environment

- Project commit: `c4646171139ee8a3c38103eaa1699dad226ec12b`
- Test commit: `c4646171139ee8a3c38103eaa1699dad226ec12b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 29.5 to 29.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 29.5 | 1 | 1 | [run](https://argusic.com/run/f83952ce-b690-4e7b-9f39-6b0d9c3e6b5e) |
| 2 | pass with mocks | 92 | 1.5 | 29.5 | 3 | 3 | [run](https://argusic.com/run/36f49f73-6773-47aa-a7ca-1de4309d8df3) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `MLX native library libmlx.so not loadable on x86_64 Linux (no Apple Silicon); also missing triton`

Attempt 2:

- 3 min: `test_alternating_kv.py and test_dflash_tree_search.py unconditionally imported mlx.core (macOS-only), preventing import-time collection on Linux`
- 4 min: `test_affine_rows.py fixture for simd_qmm was missing attributes (_HEADER, MMA_SGS, NR, RT_MAX, _DEFAULT, SCALAR_ROWS, splits/scalar_block/tiles) and simd_qmm_bits mock, causing 11 setup errors`
- 1 min: `test_affine_rows.py mx() fixture lacked mlx.core.metal.device_info and mlx.core.device_info, causing threads.py _probes() crash`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
