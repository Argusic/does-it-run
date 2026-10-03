# calico

**Verdict: could not verify.** Argusic Score 71.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/projectcalico/calico, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/calico

## Pinned environment

- Project commit: `69a6d85fdba312197207411a2542c81c1bae7db6`
- Test commit: `69a6d85fdba312197207411a2542c81c1bae7db6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 30.1 to 56.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 62.22 | 43 | 56.7 | 9 | 1 | [run](https://argusic.com/run/8871bd60-af3a-45d5-a906-b49112782453) |
| 2 | fail | 80 | 29 | 30.1 | 6 | 6 | [run](https://argusic.com/run/c0c90b1f-8068-40fa-87b2-27cd292b00bf) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27.1 not installed in container`
- `operator build fails: missing gateway-helm.tgz and base.tgz helm chart archives`
- `kube-controllers envtest tests fail: missing /usr/local/kubebuilder/bin/etcd binary`
- `libcalico-go lib/backend/k8s/resources IPAM tests fail: missing KUBECONFIG`
- `libcalico-go lib/validator/v3 tier validation tests fail: missing KUBECONFIG`
- `api/pkg/apis/projectcalico/v3 BGPFilter tests fail: missing KUBECONFIG`
- `node/tests/k8st and node/pkg/status tests fail: missing KUBERNETES config`
- `felix CGO packages fail: missing libbpf.h and pcap.h system headers`
- `Makefile build system requires Docker which is not available in container`

Attempt 2:

- 2 min: `Go 1.27.1 not pre-installed in container`
- 5 min: `libcalico-go/lib/validator/v3: 6/704 tests fail needing /kubeconfig.yaml (kubernetes backend e2e)`
- 2 min: `cni-plugin/pkg/install: 14/22 tests fail needing Docker + k8s cluster`
- 1 min: `api/pkg/apis/projectcalico/v3: 7 BGPFilter tests fail needing k8s config`
- 2 min: `felix: cannot build , missing libbpf.h and pcap.h system headers`
- 1 min: `typha: no standalone main.go in cmd/typha (NewCommand is integrated into calico-node binary)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
