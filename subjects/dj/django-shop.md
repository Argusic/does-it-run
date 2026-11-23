# django-shop

**Verdict: runs.** Argusic Score 98.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/awesto/django-shop, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/django-shop

## Pinned environment

- Project commit: `951d1e75b1f44aeb17f136cd9641b97bfeb12d14`
- Test commit: `951d1e75b1f44aeb17f136cd9641b97bfeb12d14`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.6 to 44.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96.67 | 35 | 44.7 | 6 | 5 | [run](https://argusic.com/run/cf3ae804-1062-41e5-b3f9-b62f44c9f2cf) |
| 2 | pass | 100 | 3 | 4.6 | 5 | 5 | [run](https://argusic.com/run/22993021-7368-415c-bc19-e605bd930c38) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `email_auth/models.py: ugettext_lazy removed in Django 4.x`
- 22 min: `shop/signals.py: providing_args removed from Signal`
- 28 min: `shop/payment/providers.py: ForwardFundPayment init checks OrderModel too early`
- 30 min: `shop/models/order.py: @transaction.atomic decorator incompatible with Python 3.12`
- 32 min: `shop/money/money_maker.py: Money __eq__ and _assert_addable raise on non-Money comparisons`
- 34 min: `tests/test_order.py::test_fulfill_order_partially: status mismatch (ship_goods vs ready_for_delivery) from django-fsm version incompatibility`

Attempt 2:

- 1 min: `pip install failed: externally-managed-environment (PEP 668) prevents system-wide install`
- 1 min: `Old django-allauth 0.40.0 fails to build with modern setuptools: ImportError cannot import name 'convert_path'`
- 1 min: `lxml 4.5.0 fails to compile on python3.12 (missing C headers)`
- 1 min: `pytest 5.3.1 crashes on Python 3.12: AttributeError: __spec__ from old py package`
- 1 min: `urllib3 1.25.9 missing packages.six.moves module`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
