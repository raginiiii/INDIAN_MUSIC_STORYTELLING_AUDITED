# 10 — UX and Interaction Architecture

## Information architecture
- Home / introduction
- Guided storytelling
- Tradition explorations
- Instrument discovery and detail
- Craftsmanship journey
- Maker and musician stories
- Cultural context
- Interactive exploration
- Sound and media archive
- Sources and credits

## Primary user journeys
### Curious visitor
Home → opening story → place/material → instrument → anatomy → sound → cultural context.

### Instrument enthusiast
Instrument explorer → instrument detail → anatomy → craft → playing technique → recording → related instruments.

### Craft/culture explorer
Material or craft entry → instrument → making process → maker → knowledge transmission → sources.

## Interaction specifications

### Geographical exploration
- Intent: discover instrument and tradition relationships to place.
- Entry: Explore / Made by Place.
- Action: select region or marker.
- Response: show supported associated records and uncertainty.
- Information: region, tradition, instruments, sources.
- States: default, hover, selected, loading, empty, error.
- Exit: clear or change selection.
- Mobile: tap-first, with searchable/list alternative.
- Accessibility: keyboard-accessible region list and text equivalent; map is not the only route.

### Instrument anatomy
- Intent: understand components and their function.
- Entry: instrument detail.
- Action: select labelled hotspot or component list item.
- Response: highlight component and reveal details.
- Information: name, material, function, sound contribution, source.
- States: idle, focus, selected, unavailable.
- Exit: select another part or close panel.
- Mobile: tap hotspot or list; show details in bottom sheet.
- Accessibility: equivalent ordered list; labels must not rely on colour alone.

### Craft process
- Intent: understand how an instrument is made.
- Entry: craft section or instrument detail.
- Action: scroll through or select process stages.
- Response: update stage image, description and progress.
- Information: materials, tools, technique, stage-specific source.
- States: upcoming, active, selected, unavailable.
- Exit: continue, select another stage or return to overview.
- Mobile: vertical sequence; no pinned horizontal scroll requirement.
- Accessibility: complete linear text sequence; motion optional.

### Material comparison
- Intent: compare documented materials and uses.
- Entry: materials explorer.
- Action: select two materials or material uses.
- Response: side-by-side or stacked comparison.
- Information: properties, instrument use, component use and sources.
- States: unselected, selected, comparing, unavailable.
- Exit: remove selection or reset.
- Mobile: stacked comparison or tabs.
- Accessibility: semantic table/list alternative.

### Sound player
- Intent: hear a sourced recording.
- Entry: instrument or sound archive.
- Action: play, pause, seek or change recording.
- Response: one global player updates.
- Information: recording title, performer, instrument, context, source and licence/permission status.
- States: idle, loading, playing, paused, ended, error, unavailable.
- Exit: pause or select another recording.
- Mobile: compact persistent player where it does not obscure content.
- Accessibility: keyboard controls, announced state, seek labels and transcript/context where available.
- Rule: never autoplay.

### Maker–musician connections
- Intent: understand documented human relationships.
- Entry: people or instrument page.
- Action: select a profile or relationship.
- Response: show only evidence-backed links.
- Information: role, biography, workshop/performance context and source.
- States: default, selected, connected, unavailable.
- Exit: return to origin or select another profile.
- Mobile: stacked profile and relationship list.
- Accessibility: textual relationship descriptions; do not rely on graph lines.

### Tradition switching
- Intent: compare or move between traditions.
- Entry: tradition selector.
- Action: select a tradition.
- Response: update related content and context.
- States: default, selected, loading, unavailable.
- Exit: return to index or choose another.
- Mobile: select control or horizontally scrollable tabs.
- Accessibility: selected state announced; keyboard operable.

### Related instruments
Show connections only when a typed relationship and supporting evidence exist. Explain why two instruments are related.

### Archive media viewer
- Intent: inspect an image or video and its context.
- Entry: image, archive or profile.
- Action: open viewer.
- Response: show media, caption, creator, date, source and licence.
- States: loading, displayed, unavailable, error.
- Exit: close, Escape, or return focus to trigger.
- Mobile: full-screen viewer.
- Accessibility: descriptive alt text, captions, keyboard controls and focus management.

## Overlay patterns
1. Information drawer for component/person/context detail.
2. Full-screen media viewer for images and video.
3. Comparison drawer for two or more records.

Avoid nested overlays. Trap focus in modal dialogs, close with Escape, and restore focus to the invoking control.

## Navigation
Sticky compact header with logo, Explore, Traditions, Instruments, Archive and About/Sources. Mobile uses an accessible menu drawer. Include breadcrumbs or a clear return path on detail views.

## Responsive rules
- Mobile: below 640 px.
- Tablet: 640–1023 px.
- Desktop: 1024 px and above.
These are starting points; adjust to content needs. Design mobile interactions intentionally, not as compressed desktop layouts.

## Accessibility
Target WCAG 2.2 AA. Use semantic HTML, visible focus, logical heading order, keyboard support, contrast checks, reduced-motion support, captions/transcripts where available, descriptive alt text and non-visual alternatives for maps/diagrams. Touch targets should ideally be at least 44×44 CSS pixels.
