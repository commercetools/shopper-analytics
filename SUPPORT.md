# Support

Thanks for taking a look at Shopper Analytics. It is commercetools-labs reference code: shared in
the hope that it is useful, and **unsupported**.

In practice that means:

- It is freely available under the MIT license ([LICENSE](LICENSE)) and is provided as-is, without
  warranty.
- It isn't covered by commercetools Support, your account team or any service-level agreement, so
  we can't promise replies, fixes or new releases.
- Issues and pull requests are welcome, and we'll take a look when we can.

## When something does not work

The answer to most problems is already in the admin, the docs or the test suite:

- **Install health** in the admin lists every event the collector refused, with the reason. Most
  "the reports are empty" questions are answered there.
- The [troubleshooting section](docs/gcp-setup.md#troubleshooting) of
  [docs/gcp-setup.md](docs/gcp-setup.md) covers the failures that come up most often: unregistered
  site slugs, origin mismatches, missing result counts, and Cloud SQL connection strings.
- `npm test` runs the whole suite offline against a scratch database. If it passes and your
  deployment misbehaves, the difference is in configuration.

## Before you go to production

Read [docs/privacy.md](docs/privacy.md), set per-site origins, and turn on retention. Those three
are the decisions the module deliberately leaves to you.

## If you need help

- **Questions and bugs:** open a GitHub issue. Another reader or a maintainer may well have an
  answer, though we can't commit to one.
- **Using it in production:** feel free to fork it and adapt it to your needs. Once it's in
  production it's yours, so review the code, test it against your own sites and keep your copy up
  to date.
- **commercetools products:** for questions about Composable Commerce or the Merchant Center
  themselves, the [commercetools documentation](https://docs.commercetools.com), the community and
  commercetools Support are the right place, as usual.
