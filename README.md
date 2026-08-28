---
license: cc-by-4.0
pretty_name: Stremio Addons Directory & Metadata Dataset
task_categories:
- text-classification
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

This dataset contains 553 approved public records exported from [addons-stremio.com](https://addons-stremio.com/dataset) on 2026-08-28T18:30:15.127Z.

It is generated automatically from the public directory catalog and mirrored for discovery, research, and integration use.

## Files

- `addons.json` / `stremio-addons.json`: complete nested export with dataset metadata.
- `stremio-addons.jsonl`: one addon record per line.
- `addons.csv` / `stremio-addons.csv`: flattened fields for analysis.
- `forum-threads.json`: complete public forum export with published replies and equivalent-language links.
- `forum-threads.jsonl`: one redacted public forum thread per line.
- `forum-threads.csv`: flattened public forum records for analysis.
- `metadata.json`: generation timestamp, record count, source links, and checksum.

## Main schema

Core addon fields include `id`, `stremioId`, `slug`, `name`, `description`, `version`, `canonicalUrl`, `manifestUrl`, `types`, `categories`, `languages`, `health`, `community`, `provenance`, and `updatedAt`.

## Scope and provenance

Records include public manifest URLs, canonical directory URLs, descriptions, taxonomy, language tags, health timestamps, community signals, and publication dates. Private account, ownership, moderation, fingerprint, developer email, and internal discovery-source fields are excluded.

Forum records include only published threads that meet the directory's substantive-content threshold. Author names, account identifiers, votes, reports, ownership fields, and moderation data are excluded; contact-like text is redacted. Each forum record links to its canonical page, category, related addon (when applicable), replies, and equivalent-language threads (when published).

Manifest availability does not guarantee every independent catalog, stream, subtitle, provider, or geographic region. The directory does not host addon media.

## Live API

The current API is documented at [addons-stremio.com/openapi.yaml](https://addons-stremio.com/openapi.yaml).
The dataset landing page is [addons-stremio.com/dataset](https://addons-stremio.com/dataset), and the public catalog API is [addons-stremio.com/api/v1/addons](https://addons-stremio.com/api/v1/addons).
The public forum API is [addons-stremio.com/api/v1/forum/threads](https://addons-stremio.com/api/v1/forum/threads), and new discussions are available in the [forum Atom feed](https://addons-stremio.com/forum/feed.xml).

## License

Dataset compilation and directory annotations are available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Third-party names, icons, manifests, and descriptions remain subject to their respective owners and terms.
