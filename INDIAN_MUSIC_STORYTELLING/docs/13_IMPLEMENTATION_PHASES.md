# 13 — Implementation Phases

## Phase 0 — Research readiness
- Restore the approved tradition list.
- Obtain original Indian research datasets and notes.
- Build source and verification records.
- Populate and validate normalized data.
- Confirm media rights.
**Gate:** no tradition-specific UI content until core records have sources.

## Phase 1 — Project foundation
- Initialise React, TypeScript and Vite.
- Configure linting, formatting and routing.
- Establish folder structure and providers.
- Add design tokens and font fallbacks.
**Acceptance:** app builds, routes load, no console errors.

## Phase 2 — Design system
- Header, footer, buttons, typography, cards, drawers, modals and image fallbacks.
- Responsive layout primitives.
- Focus, hover, active, disabled and error states.
**Acceptance:** components work on keyboard and mobile.

## Phase 3 — Data integration
- Define TypeScript types and validation.
- Load JSON records.
- Resolve relationships by stable ID.
- Display data-status and source references in development mode.
**Acceptance:** invalid references are detected; no silent fallback facts.

## Phase 4 — Editorial narrative
- Homepage and guided story sections.
- Tradition overview templates.
- Progressive disclosure patterns.
**Acceptance:** story remains coherent with reduced motion and no audio.

## Phase 5 — Independent exploration
- Instrument index and search.
- Geography/material entry points where data supports them.
- Related-instrument links.
**Acceptance:** all displayed relationships resolve to valid records.

## Phase 6 — Deep interactions
- Anatomy explorer.
- Craft process sequence.
- Material comparison.
- Maker and musician profiles.
**Acceptance:** each control reveals the correct record and has an accessible alternative.

## Phase 7 — Sound and media
- Global audio controller.
- Approved embeds.
- Media viewer and credits.
- Fallbacks and loading states.
**Acceptance:** no autoplay; unavailable media does not break page content.

## Phase 8 — QA and optimisation
- Responsive testing.
- WCAG review.
- Performance and broken-link checks.
- Content/source audit.
**Acceptance:** checklist in `15_QA_AND_VALIDATION.md` passes.

## Phase 9 — Deployment
- Production build.
- Environment and secrets review.
- Hosting configuration.
- Final smoke test and source/credit review.
**Acceptance:** deployment works and all published assets have verified rights status.

## Development discipline
Implement in small phases. Do not replace existing working features while adding new ones. After each phase, run the build, inspect browser console, test keyboard interactions and review mobile layout.
