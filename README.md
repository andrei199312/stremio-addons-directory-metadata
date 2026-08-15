---
license: cc-by-4.0
pretty_name: Stremio Addons Directory & Metadata Dataset
task_categories:
- text-retrieval
- feature-extraction
language:
- en
size_categories:
- n<1K
tags:
- stremio
- addons
- streaming-metadata
---

# Stremio Addons Directory & Metadata Dataset

This dataset contains 507 approved public records exported from [addons-stremio.com](https://addons-stremio.com/dataset) on 2026-08-15T00:37:02.855Z.

## Files

- `stremio-addons.json`: complete nested export with dataset metadata.
- `stremio-addons.jsonl`: one addon record per line.
- `stremio-addons.csv`: flattened fields for analysis.

## Scope and provenance

Records include public manifest URLs, canonical directory URLs, descriptions, taxonomy, language tags, health timestamps, community signals, publication dates, and source-directory provenance when available. Private account, ownership, moderation, fingerprint, and developer email fields are excluded.

Manifest availability does not guarantee every independent catalog, stream, subtitle, provider, or geographic region. The directory does not host addon media.

## Live API

The current API is documented at [addons-stremio.com/openapi.yaml](https://addons-stremio.com/openapi.yaml).

## License

Dataset compilation and directory annotations are available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Third-party names, icons, manifests, and descriptions remain subject to their respective owners and terms.
