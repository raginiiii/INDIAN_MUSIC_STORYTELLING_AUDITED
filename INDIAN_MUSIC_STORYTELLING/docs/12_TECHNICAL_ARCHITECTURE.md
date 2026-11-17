# 12 — Technical Architecture

## Recommended stack
- React + TypeScript.
- Vite for the initial Google AI Studio React project.
- Tailwind CSS plus custom CSS design tokens.
- Motion for purposeful transitions.
- SVG and D3.js only for custom, evidence-backed visualisations.
- Lightweight SVG/GeoJSON mapping where geography warrants it.
- React Router for content routes.
- React Context for shared exploration, overlay and audio state.
- Local JSON for curated research data.
- HTML5 Audio for permitted local audio; official/approved embeds where required.
- Responsive image assets with fallbacks.
- Lucide React for interface icons.

This is a recommended implementation choice, not a claim that Next.js is unsuitable. Reassess Next.js if server rendering, extensive SEO, server-side content management or a larger production platform becomes necessary.

## Architecture principles
- Separate content data from UI components.
- Keep datasets outside component files.
- Use stable IDs and typed relationships.
- Avoid unnecessary external APIs.
- Avoid runtime AI-generated facts.
- Do not fetch remote content on every page visit when verified local data is sufficient.
- Keep media handling separate from content entities.
- Validate JSON against TypeScript types or a runtime schema.

## Suggested project structure
```text
src/
  app/                 # app bootstrap, routes, providers
  pages/               # Home, Explore, Tradition, Instrument, Craft, People, Sources
  components/
    layout/
    storytelling/
    instruments/
    geography/
    craft/
    people/
    audio/
    media/
    ui/
  data/                # imports or loaders for JSON
  context/             # exploration, audio, overlay
  hooks/
  types/
  utils/
  styles/
public/
  images/
  audio/
  video/
  fonts/
```

## Data architecture
Entities: traditions, geography, instruments, makers, materials, craft processes, musicians, media and sources. Relationships are many-to-many where appropriate. Use separate relationship IDs or arrays of stable foreign keys. Every content entity should carry `sourceIds` and a `dataStatus`.

## State
Shared state:
- selected tradition, region and instrument;
- selected anatomy component;
- comparison selections;
- active recording and playback state;
- active overlay;
- search query and filters.

Keep ephemeral state local to components. Put shareable filters/selections in URL parameters where useful.

## Routing
Suggested:
- `/`
- `/explore`
- `/traditions`
- `/traditions/:traditionId`
- `/instruments`
- `/instruments/:instrumentId`
- `/makers/:makerId`
- `/musicians/:musicianId`
- `/craft`
- `/sound`
- `/sources`

A single-page narrative may still use routes for shareable detail states. Do not duplicate entity content across pages.

## Component architecture
Reusable components receive typed records through props. They must not embed large datasets or factual copy. Build shared layout, cards, drawers, media viewers, selectors and player before complex visualisations.

## Media
One global audio controller; one active recording at a time. Lazy-load video embeds and below-the-fold images. Do not autoplay. Handle missing media gracefully.

## Animation
Use transform/opacity where possible. Respect `prefers-reduced-motion`. Avoid scroll hijacking, excessive parallax and animations that block content. Sound-reactive visuals must use actual accessible audio analysis or be labelled illustrative.

## Accessibility
Semantic HTML, keyboard support, visible focus, focus management, captions/transcripts where available, reduced motion, alt text and text equivalents for visualisations.

## Performance
Use responsive images, modern formats, lazy loading, code splitting for heavy modules, on-demand media loading and limited dependencies. Test on representative mobile hardware and slower connections.

## Error handling
All interactive modules need loading, success, empty/unavailable and error states. A map falls back to a region list; anatomy falls back to a labelled component list; audio falls back to metadata and source link; craft sequence remains readable without imagery or animation.

## Security and privacy
Do not put API keys or secrets in client code. Avoid collecting personal data. If a future API is introduced, document purpose, data flow, rate limits, privacy and failure modes.
