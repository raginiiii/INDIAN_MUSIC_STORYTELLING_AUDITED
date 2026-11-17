# 15 — QA and Validation

## Research integrity
- [ ] Every tradition in the interface matches the approved selection register.
- [ ] Every factual record has a stable ID.
- [ ] Every non-trivial claim has source IDs.
- [ ] Every relationship resolves to an existing record.
- [ ] Unknown, partial and disputed data are labelled accurately.
- [ ] No invented people, instruments, origins, dates or craft stages.
- [ ] Community terminology and transliteration reviewed.
- [ ] Sensitive knowledge and interview consent reviewed.

## Media
- [ ] Asset source page recorded.
- [ ] Creator and attribution recorded.
- [ ] Licence/permission verified for intended use.
- [ ] Crop/derivative permission checked.
- [ ] Audio/video embed method is permitted.
- [ ] Alt text and captions/transcripts provided where possible.
- [ ] Fallback works when media fails.

## Functionality
- [ ] Navigation and routes work.
- [ ] Search returns valid records only.
- [ ] Filters can be cleared.
- [ ] Map has a text alternative.
- [ ] Anatomy hotspots and component list remain in sync.
- [ ] Craft process can be explored without scroll animation.
- [ ] Comparison shows only supported attributes.
- [ ] Audio play/pause/seek/switch/error states work.
- [ ] Drawers and modals close with Escape.
- [ ] Focus returns to the invoking control.
- [ ] No autoplay.

## Responsive
- [ ] 320 px width and common mobile widths.
- [ ] Tablet layouts.
- [ ] Desktop and large desktop.
- [ ] No horizontal overflow.
- [ ] Touch targets are sufficiently large.
- [ ] Bottom sheets and menus do not obscure essential controls.

## Accessibility
- [ ] WCAG 2.2 AA contrast review.
- [ ] Keyboard-only navigation.
- [ ] Visible focus.
- [ ] Semantic headings and landmarks.
- [ ] Screen-reader labels and status announcements.
- [ ] Reduced-motion mode.
- [ ] Text alternatives for maps, diagrams and waveforms.
- [ ] Captions/transcripts where available.

## Performance
- [ ] Images responsive and lazy-loaded appropriately.
- [ ] Video embeds load on demand.
- [ ] Audio loads only when requested.
- [ ] Heavy modules code-split where useful.
- [ ] No avoidable layout shifts.
- [ ] Test on representative mobile device and constrained connection.
- [ ] Production build succeeds.

## Release gate
Do not publish if source provenance, rights, or core factual accuracy remain unresolved. Record any accepted limitations in the verification log.
