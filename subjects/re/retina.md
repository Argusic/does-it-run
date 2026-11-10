# retina

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/retina, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/retina

## Pinned environment

- Project commit: `8945309e622b31c6eb0f7cd837c2ef8c111a5670`
- Test commit: `8945309e622b31c6eb0f7cd837c2ef8c111a5670`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 32.4 to 36 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 35 | 36 | 6 | 4 | [run](https://argusic.com/run/41e9f3b0-d893-4a73-b4d4-718740bfde16) |
| 2 | pass | 100 | 32 | 32.4 | 3 | 3 | [run](https://argusic.com/run/e9afdf6f-3c35-424b-9ac5-ddcb7d7531e9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Go compiler in container`
- 0.5 min: `llvm-strip not found (needed for eBPF .o stripping)`
- 3 min: `clang not found (needed for eBPF C→.o compilation via bpf2go)`
- 0.5 min: `LLVM 18 clang requires libtinfo.so.5 which is not on system`
- `retinaendpoint BeforeSuite fails: no etcd at /usr/local/kubebuilder/bin/etcd`
- `loader vmlinux_linux_test fails: bpftool not in PATH`

Attempt 2:

- 3 min: `Go not installed in environment`
- 5 min: `pkg/loader: TestGenerateVmlinuxH fails - bpftool not found`
- 5 min: `pkg/controllers/daemon/retinaendpoint: needs etcd for kubebuilder test env`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
