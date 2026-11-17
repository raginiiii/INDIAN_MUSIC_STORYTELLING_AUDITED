# Indian Music Storytelling — Research & Development Pack

**Project status:** Architecture and visual direction documented; tradition-level research and verified content datasets are not present in the available source materials.

This archive is organised for handoff to Google AI Studio. It contains the approved project direction, narrative and UX architecture, implementation specification, data contracts, research and media manifests, validation rules, and an explicit record of missing evidence.

## Start here
1. `docs/00_START_HERE.md`
2. `docs/01_PROJECT_BRIEF.md`
3. `docs/08_VISUAL_DIRECTION.md` and `docs/09_DESIGN_SYSTEM.md`
4. `docs/10_UX_AND_INTERACTION.md`
5. `docs/12_TECHNICAL_ARCHITECTURE.md`
6. `docs/14_AI_STUDIO_MASTER_PROMPT.md`

## Important research integrity notice
The available uploaded PDF is a Beatles discography/storytelling dossier, not an Indian musical-instrument dataset. It has deliberately not been used as evidence or copied into this package. No Indian instrument, maker, musician, tradition, media asset or source record has been fabricated to make the package appear complete.

The approved project context establishes a human-centred journey through Indian instruments, makers, craftsmanship and cultural significance, with approximately 6–8 traditions explored deeply. The exact approved tradition list and underlying research records were not present in the accessible source material at package-generation time. See `research/research_gaps.md`.

## Folder map
- `docs/` — project, research, narrative, visual, UX and technical specifications.
- `data/` — typed, currently empty datasets and a data dictionary.
- `media/` — asset manifests and credit rules.
- `research/` — source registers, gap log and verification log.
- `original_data/` — untouched source inputs. Currently contains an explanatory README because no Indian project source dataset was available.

## Data status
All JSON files are valid JSON arrays with zero records. They are intentionally empty, not sample content. Add only evidence-backed records with stable IDs and source references.

## Google AI Studio
Upload the extracted folder as project context. Use `docs/14_AI_STUDIO_MASTER_PROMPT.md` as the master instruction. Do not ask the coding agent to invent missing research or media.


## Independent research audit

Read `docs/17_INDEPENDENT_RESEARCH_AUDIT.md` and `research/independent_audit_register.csv` before using this package. The research corpus is not ready for factual-content implementation or publication; see the audit's readiness gates.
