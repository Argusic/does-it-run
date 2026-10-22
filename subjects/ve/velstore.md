# velstore

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/velstorelabs/velstore, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/velstore

## Pinned environment

- Project commit: `c1c32c7b9f1eb2fc20deb449a019c84b0e6ab3ba`
- Test commit: `c1c32c7b9f1eb2fc20deb449a019c84b0e6ab3ba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 18.6 to 58.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 18.6 | 0 | 0 | [run](https://argusic.com/run/6b0dcf43-a146-4ccb-8db2-872fa8000fc4) |
| 2 | pass | 100 | 58 | 58.8 | 8 | 8 | [run](https://argusic.com/run/44099e7c-3f00-4629-9c20-bc3efb9a1599) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `No PHP interpreter present in container`
- 3 min: `Composer refused install: ext-tokenizer/fileinfo/xmlwriter reported missing`
- 4 min: `composer install post-autoload failed: 'Class [config] does not exist' ReflectionException loop`
- 4 min: `Admin PaymentGatewayConfigController imported in routes but file did not exist (route:list and /admin/payment_gateway_configs 500)`
- 6 min: `Vendor SocialMediaLinkController referenced but missing and its repo was unbound`
- 5 min: `Vendor products 500: App\Services\vendor\ProductService wrong case and repo in lowercase app/Repositories/Vendor/product/ violated PSR-4`
- 10 min: `Store checkout 500: Order wrote user_id/address/payment_method/total to columns that did not exist, and OrderItem/ShippingAddress models and thankyou route were missing`
- 4 min: `PaymentGateway seeder used key names client_secret/public_key/secret_key and was not idempotent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
