# 14 — Google AI Studio Master Prompt

You are implementing **Beyond the Sound**, an editorial interactive archive about selected Indian musical instruments, their makers, craftsmanship, musicians and cultural contexts.

## Mandatory research audit gate
Read `docs/17_INDEPENDENT_RESEARCH_AUDIT.md` and `research/independent_audit_register.csv` before coding. The current research corpus is NOT ready for factual-content implementation. Build only the visual system, navigation, reusable components, empty states and schema/test infrastructure until the readiness gates in the audit pass. Never populate factual pages from model knowledge.

## Read before coding
Read the entire project pack, especially:
- `README.md`
- `docs/01_PROJECT_BRIEF.md`
- `docs/02_RESEARCH_METHODOLOGY.md`
- `docs/03_TRADITION_SELECTION.md`
- `docs/04_RESEARCH_DOSSIER.md`
- `docs/05_INSTRUMENT_DATABASE.md`
- `docs/06_DATA_STORYTELLING.md`
- `docs/07_NARRATIVE_ARCHITECTURE.md`
- `docs/08_VISUAL_DIRECTION.md`
- `docs/09_DESIGN_SYSTEM.md`
- `docs/10_UX_AND_INTERACTION.md`
- `docs/11_MEDIA_AND_ASSET_GUIDELINES.md`
- `docs/12_TECHNICAL_ARCHITECTURE.md`
- `docs/13_IMPLEMENTATION_PHASES.md`
- `docs/15_QA_AND_VALIDATION.md`
- `data/data_dictionary.md`
- all JSON datasets and media manifests.

## Critical truthfulness constraints
1. Do not invent traditions, instruments, makers, musicians, materials, dates, geographic origins, cultural meanings, craft steps, recordings or sources.
2. The data files are currently empty because verified Indian project datasets were not available in the handoff. Do not fill them with examples or model knowledge.
3. If data is missing, build a neutral empty state and keep the component architecture ready for later data.
4. Do not treat the unrelated Beatles PDF as a source for this project.
5. Do not use a generic stock photograph as if it depicts a named tradition, maker or instrument.
6. Do not publish media unless its rights status allows the intended use.
7. Keep research facts in data files, not hardcoded in React components.

## Design direction
Implement “The Living Archive, in Motion”: editorial, calm, tactile and immersive. Use Fraunces or Instrument Serif for display typography and a legible sans-serif for body/UI. Maintain whitespace, clear hierarchy and restrained earthy accents. Avoid generic cultural ornament, pseudo-script and excessive vintage filters. Motion and sound must serve discovery.

## Experience requirements
Support guided storytelling and independent exploration. The user should be able to enter through geography, tradition, instrument, material, craft, maker, musician or sound when records exist. Use progressive disclosure and avoid overwhelming the user.

## Technical requirements
Use React + TypeScript + Vite unless the existing AI Studio scaffold requires a compatible adjustment. Use Tailwind CSS and custom tokens, Motion for purposeful animation, SVG/D3 only where needed, React Router, React Context for shared state and local JSON for curated data. Keep components reusable and typed.

## Interaction requirements
Implement the specifications in `docs/10_UX_AND_INTERACTION.md`. Every control must have a real outcome. Provide keyboard access, visible focus, mobile-specific behaviour, reduced-motion support and textual alternatives. Never autoplay audio or video.

## Media requirements
Use a global audio controller. Lazy-load media. Provide attribution, loading, unavailable and error states. Never assume that a URL implies permission to reuse an asset.

## Implementation process
Work phase by phase using `docs/13_IMPLEMENTATION_PHASES.md`.
- First inspect the scaffold and report the current structure.
- Implement Phase 1 only.
- Show changed files and explain how to test.
- Do not proceed until the current phase builds and passes its acceptance criteria.
- Preserve working code and existing user changes.
- Avoid unnecessary dependencies and APIs.

## Definition of done
The result is not complete merely because it looks attractive. All visible interactions must work; all content must be source-backed; empty states must be intentional; mobile and keyboard behaviour must be tested; and no media or factual record may be fabricated.
