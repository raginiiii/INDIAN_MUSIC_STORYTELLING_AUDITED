# Data Dictionary

## Dataset conventions
All datasets are UTF-8 JSON objects with:
- `_meta`: dataset-level status and notes.
- `records`: array of entity records.

All current `records` arrays are empty intentionally. No sample records are included because that could be mistaken for researched content.

## ID conventions
Use stable, opaque IDs:
- `TR-###` tradition
- `IN-###` instrument
- `MK-###` maker
- `MA-###` material
- `PR-###` craft process
- `MU-###` musician
- `RG-###` geographic entity
- `MD-###` media asset
- `SR-###` source
- `CP-###` instrument component

Do not recycle IDs after publication. IDs must not encode mutable names or assumptions.

## Common fields
| Field | Type | Meaning |
|---|---|---|
| `id` | string | Stable unique identifier |
| `name` | string | Preferred display name |
| `alternateNames` | string[] | Verified alternate names |
| `description` | string | Concise sourced description |
| `sourceIds` | string[] | Foreign keys into source register |
| `dataStatus` | enum | verified, corroborated, partial, disputed, unverified, unknown |
| `notes` | string | Editorial/research caveats |

## Entity relationships
- Tradition ↔ instrument: many-to-many.
- Instrument ↔ region: many-to-many.
- Instrument ↔ material: many-to-many, ideally through component/use records.
- Instrument ↔ maker: many-to-many where documented.
- Instrument ↔ musician: many-to-many where documented.
- Instrument ↔ craft process: one-to-many or many-to-many as supported.
- All entities ↔ source: many-to-many.

Use arrays of stable IDs initially. Validate every foreign key at build time.

## Instrument recommended fields
`id`, `name`, `alternateNames`, `traditionIds`, `regionIds`, `classification`, `description`, `anatomy`, `materialIds`, `processIds`, `makerIds`, `musicianIds`, `mediaIds`, `sourceIds`, `dataStatus`.

## Component recommended fields
`id`, `instrumentId`, `name`, `alternateNames`, `materialIds`, `function`, `soundContribution`, `hotspotKey`, `mediaIds`, `sourceIds`, `dataStatus`.

## Craft process recommended fields
`id`, `instrumentIds`, `name`, `sequence`, `description`, `materialsUsed`, `toolsUsed`, `technique`, `makerIds`, `mediaIds`, `sourceIds`, `variationNotes`, `dataStatus`.

## Media references
Media entity details live in CSV manifests until a dedicated `media.json` is introduced. `mediaIds` must match manifest IDs exactly.

## Unknowns
Use `null` or omit optional fields when genuinely unknown; do not use empty strings as factual values. Use `unknown` status when absence of evidence must be made explicit. Never convert missing data into a negative claim.
