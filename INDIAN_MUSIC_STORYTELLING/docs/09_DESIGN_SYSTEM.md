# 09 — Design System

## Typography
- Display: Fraunces or Instrument Serif. Choose one as the primary display family after visual testing.
- Body/UI: Inter or another highly legible sans-serif.
- Use a consistent type scale; avoid using display serif for dense metadata.
- Self-host licensed font files where permitted; otherwise load from a documented, reliable font source with a system fallback.

## Colour
Use semantic tokens rather than hard-coded colours:
- `paper`: warm light surface;
- `surface`: card and panel surface;
- `ink`: primary text;
- `muted`: secondary text;
- `line`: subtle separators;
- `accent`: restrained terracotta / earthy accent;
- `focus`: high-visibility keyboard focus;
- `success`, `warning`, `error`: accessible status colours.

Final hex values must be selected in the design implementation and checked for WCAG AA contrast. Do not infer exact approved colour values from a text description.

## Layout
- Editorial max-width container with flexible gutters.
- Asymmetric image/text compositions where they support the story.
- Consistent spacing scale.
- Clear separation between narrative content and interactive controls.
- Avoid card grids as the default layout for every section.

## Image treatment
- Prefer documentary images with verified provenance and consent/licence.
- Use image captions and credits.
- Keep focal subjects visible across responsive crops.
- Do not use image-only text or embed essential information in images.

## Motion
- Use opacity and transform for most transitions.
- Keep interaction feedback fast and predictable.
- Avoid scroll hijacking and perpetual motion.
- Respect `prefers-reduced-motion`.
- Ensure all information is available without animation.

## Components
Buttons, tabs, cards, drawers, modals, tooltips, audio controls, image viewers and selectors must share consistent states, spacing, focus styles and responsive rules.
