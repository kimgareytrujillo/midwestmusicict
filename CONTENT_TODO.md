# Content TODO

Open items from Kim's content brief (`midwest-music-ict-content.md`), tracked here so nothing gets lost.
Search the codebase for `TODO` comments to find the exact spots.

## Open items for the client to fill in

- [ ] Final package tiers, inclusions, and pricing (`src/pages/packages.astro`)
- [ ] Phone number and email for Contact page/footer (`src/pages/contact.astro`, `src/components/SiteFooter.astro`)
- [ ] Service area / location wording (`src/pages/contact.astro`)
- [ ] Social media links (`src/components/SiteFooter.astro`)
- [ ] Testimonials, or a Google Business review link (`src/pages/index.astro`)
- [ ] Final photo selects, sorted by ensemble/event type
- [ ] Kim's real personal bio for the About page "Meet the Founder" section (`src/pages/about.astro`)

## Photos/media needed

There's no separate media page by design — photos and video should be incorporated throughout the
site, especially the Event Types page, so it can help visitors match a style/ensemble to their event.

- [ ] Hero photo — high-energy live performance shot (Home)
- [ ] Founder photo of Kim Trujillo (About, "Meet the Founder" section)
- [ ] One photo/video clip per ensemble: String Quartet, Jazz Combo, Steel Drum Band, Rock Band (Music page)
- [ ] One photo/video clip per event type: Weddings, Corporate, Private Parties, Outdoor & Themed (Event Types page)
- [ ] Gallery photos, grouped by event type if there's enough volume
- [ ] Real logo (primary mark + wide header lockup) — see placeholders on the Home page and in the header

## Functionality decisions still open

- [ ] **Contact form backend.** The form currently opens the visitor's email client with a pre-filled
      message (no backend needed). Decide whether to wire it to a real service instead — a Cloudflare
      Pages Function, or a form service like Formspree/Web3Forms — so inquiries land directly in an
      inbox or CRM.
- [ ] **Map embed** on the Contact page, if the service area or a business location should be shown.
- [ ] **Song list / repertoire page**, if Kim wants to take requests or showcase repertoire per ensemble.
      Low priority for launch.
- [ ] **Service-area landing pages** (e.g. "Wichita Wedding Band") for local SEO — worth considering once
      there's a clear primary service area and the business wants to expand reach. Not needed for launch.

## Structural notes

- The Music and Event Types pages are built from small data arrays (`ensembles` / `eventTypes` in each
  file) so new entries can be added without redesigning the page.
- Home page's "Choose Your Experience" cards and ensemble teaser grid link to anchors on the Music and
  Event Types pages (e.g. `/music/#string-quartet`) rather than literal filtering — good enough for v1.
