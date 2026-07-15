# Design System: Monetize Your Android App — Droidcon USA 2026

## 1. Visual Theme & Atmosphere

A warm, editorial conference deck with the confidence of a technical field
guide. Density is balanced at 4/10, variance is intentionally asymmetric at
7/10, and motion is restrained at 4/10. Slides should feel authored rather
than templated: large claims sit off-axis, evidence uses flat structure and
rules, and screenshots appear only when they prove the current point.

## 2. Color Palette & Roles

- **Warm Canvas** (`#F7F4EE`) — Default slide background.
- **Paper Surface** (`#FFFDF8`) — Raised screenshot and code-adjacent surface.
- **Charcoal Ink** (`#181A18`) — Primary text and dark slide background; never pure black.
- **Mineral Gray** (`#6B6E68`) — Secondary copy, metadata, and source lines.
- **Quiet Rule** (`#D7D2C8`) — Dividers and structural borders.
- **Revenue Coral** (`#E05A5F`) — The only saturated accent: emphasis, progress, arrows, and active states.
- **Coral Wash** (`#F2DDD7`) — Low-saturation section surface; not a second accent.

Blue, yellow, and green may appear inside sourced screenshots, but they are not
part of the deck chrome or semantic hierarchy.

## 3. Typography Rules

- **Display and headings:** Outfit, semibold or bold, tightly tracked with a controlled scale.
- **Body:** Outfit Regular, relaxed leading, with short lines and no paragraph wider than roughly 65 characters.
- **Code and metadata:** JetBrains Mono Regular; ExtraBold only for small labels and numbering.
- **Minimums:** 50pt deck title, 35pt slide title, 24pt callout header, 16pt body in PowerPoint.
- **Banned:** Inter, generic system-only stacks, generic serif fonts, and size-only hierarchy.

## 4. Presentation Components

- **Claims:** Left-aligned, off-axis, and paired with one typographic marker or evidence object.
- **Screenshots:** One clear crop per claim, with a warm diffused shadow and no decorative device frame.
- **Code:** Charcoal panel, JetBrains Mono, syntax color limited to coral, warm white, muted gray, and a restrained cyan only when needed for functions.
- **Cards:** Used only when grouping changes meaning. Prefer border-top rules and negative space.
- **Metrics:** Flat, large-number evidence with one coral rule; never dashboard widgets.
- **QR:** Quiet audience utility. It floats only when requested with `Q` and remains static on the closing slide.

## 5. Layout Principles

- Use a 12-column mental grid with equal outside margins and clear spatial zones.
- Prefer split screens, offset whitespace, and one dominant region.
- Avoid centered statement slides and repeated equal-card rows.
- A comparison may use repeated columns only when the repetition is the evidence.
- Keep title, proof, and implication visually distinct; do not stack decorative layers.
- Preserve 16:9 stage readability and cleanly collapse multi-column layouts on narrow screens.

## 6. Motion & Interaction

- Reveal hierarchy with a short stagger: kicker, title, evidence, then detail.
- Animate only `transform` and `opacity` with a weighty ease-out curve.
- Keep the QR utility on a subtle floating loop while visible.
- Respect `prefers-reduced-motion`; no animation is required for comprehension.
- No bouncing prompts, neon glows, custom cursors, or perpetual decorative motion.

## 7. Anti-Patterns (Banned)

- No Inter, pure black, neon gradients, or multi-accent slide chrome.
- No centered hero or centered statement pattern.
- No generic three-card feature rows or repeated UI-panel grids.
- No overlapping text and images.
- No emojis, filler prompts, fake metrics, or AI-copy clichés.
- No shrinking important copy to compensate for weak editing.
- No motion that competes with the speaker.
