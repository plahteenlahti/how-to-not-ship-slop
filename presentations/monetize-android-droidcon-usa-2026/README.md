# Monetize your Android app the right way

Droidcon USA 2026 conference deck by Perttu Lähteenlahti.

- `index.html` — browser presentation with keyboard navigation, speaker notes, and a `Q`-toggleable audience QR code
- `presentation.pptx` — editable PowerPoint export
- `DESIGN.md` — semantic design system for the browser deck
- `assets/` — presentation images and locally hosted fonts
- `assets/siivous.mp4` — Perttu's three-user cleaning app demo, reused from the earlier “How to not ship slop” talk
- `assets/netli-icon.jpg` and `assets/seo-console-icon.jpg` — official App Store artwork used on the personal products slide
- `assets/*-tight.png` — display-only crops that remove empty canvas around selected source images; archived PDF extractions remain untouched
- `assets/pdf-extracted/transparent/` — exact embedded PDF artwork with original transparency masks preserved
- `assets/pdf-extracted/opaque-originals/` — exact embedded screenshots, photos, and QR codes whose backgrounds are part of the source pixels
- `assets/pdf-extracted/manifest.json` — source page, dimensions, transparency, and deduplication metadata
- `assets/pdf-extracted/transparent-images.zip` — the 18 transparent originals as a convenient download bundle
- `assets/pdf-extracted/transparent-contact-sheet.png` — a labeled preview of the transparent set
- `source/original-deck.pdf` — the source presentation supplied for this revision
- `sources.md` — current references used for the 2026 update

The deck is designed for a roughly 35–40 minute talk plus questions.

When served locally, the QR opens the public article and code resources. When
deployed, it opens the current slide; set `CONFIGURED_DECK_URL` in `index.html`
if the public deck URL differs from the browser origin.
