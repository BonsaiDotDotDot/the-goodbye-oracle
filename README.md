# The Goodbye Oracle

Data releases for the [Buy or Goodbye](https://github.com/BonsaiDotDotDot) ecosystem.

This repository contains **no source code** — only versioned data releases published automatically by the pipeline.

## What's Here

- **GitHub Releases** — each release contains:
  - `master.sqlite` — full normalized product database
  - `master.sqlite.sig` — Ed25519 signature
  - `delta-X-to-Y.json` — changelog from previous version (when available)
  - `delta-X-to-Y.sha256` — checksum
  - `delta-X-to-Y.json.sig` — Ed25519 signature
- **`latest.json`** — manifest pointing to the most recent release

## Data Sources

This dataset is built from the following public sources:

- [Open Food Facts](https://world.openfoodfacts.org/) — product, brand, and ingredient data (Open Database License)
- [Wikidata](https://www.wikidata.org/) — corporate ownership chains (CC0)
- [US Department of Labor ILAB](https://www.dol.gov/agencies/ilab/reports/child-labor/list-of-goods) — child and forced labor goods list (public domain)
- [Leaping Bunny](https://www.leapingbunny.org/) — cruelty-free certified brands (Leaping Bunny Standard)

## Verification

All release artifacts are signed with Ed25519. The mobile app verifies signatures before applying updates.

## License

The data in this repository is licensed under [CC BY 4.0](LICENSE). See the individual data sources above for their respective licenses.
