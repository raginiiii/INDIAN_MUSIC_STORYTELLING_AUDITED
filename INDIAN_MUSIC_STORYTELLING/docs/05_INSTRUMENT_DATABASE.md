# 05 — Instrument Database

## Purpose
Define a normalized instrument catalogue that can support the instrument index, detail pages, anatomy hotspots, material comparison, related-instrument discovery and audio links.

## Record requirements
Each instrument must have a stable ID, preferred display name, alternate names where verified, tradition and region relationships, classification evidence, description, component list, material links, craft-process links, people links, media links and source references.

## Naming
Preserve the preferred local name and script where available. Store transliteration separately. Do not silently standardise spellings without recording the source form and editorial decision.

## Anatomy
Components are separate entities. Each component record should identify the parent instrument, component name, position or hotspot key, material links, physical function, sound contribution if evidenced, explanatory text and sources.

## Related instruments
Relationships must be explicit and typed, for example:
- shared material;
- comparable sound-producing mechanism;
- related playing technique;
- documented historical/cultural connection;
- shared musical context.

Do not infer a relationship from superficial visual similarity.

## Data status
`data/instruments.json` and the related component data are currently empty because no verified Indian instrument dataset was available. Do not create example instruments to fill the catalogue.
