# Contributing

Use Node 22+, `npm ci`, and `npm run validate`. Keep changes focused and include a failing regression test for bugs. Preserve protocol compatibility, schema validation, approval gates, account isolation and nutrition provenance. Use synthetic fixtures only. Do not add credentials, personal data, recordings or service exports.

Open a GitHub issue for a reproducible code problem, then a pull request describing the change and checks. Security reports follow SECURITY.md. No CLA is required.

This public integration was exported without private Git history. Runtime source and tests originate in the ReceiptCal integration package; the private backend is not required for local tests. Server-route parity is additionally checked by the private product repository and is not claimed by standalone validation. Public changes must be reconciled with the product integration before the hosted service is updated.

Maintain matching package and plugin versions. Release tags use semantic versions, with notes, a source bundle and SHA-256 checksums. Never replace an existing release asset silently; publish a new patch version. Hosted service deployment is separate from publishing this connector.

## License and sign-off

This project is licensed under the [Apache License 2.0](LICENSE). Under section 5 of that license, any contribution you intentionally submit is provided under the same Apache-2.0 terms (inbound = outbound), including its patent grant.

Every commit must carry a [Developer Certificate of Origin](https://developercertificate.org/) sign-off, certifying that you wrote the change or otherwise have the right to submit it under this license. Add it with `git commit -s`, which appends:

```
Signed-off-by: Your Name <you@example.com>
```

Use your real name. Pull requests with unsigned commits will be asked to amend them (`git commit --amend -s` or `git rebase --signoff main`). Do not change the [NOTICE](NOTICE) attribution or use the ReceiptCal name for forks; see [TRADEMARKS.md](TRADEMARKS.md).
