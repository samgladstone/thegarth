# Implementation Plan

## Phase 1 – Foundation

**Goal:** Working site skeleton deployed to Vercel.

- Initialise Astro project with Tailwind CSS
- Set up GitHub repo and connect to Vercel
- Deploy a placeholder page to confirm the pipeline works
- Configure basic meta tags (title, description, Open Graph)

**Done when:** A live URL exists on Vercel.

---

## Phase 2 – Core Content

**Goal:** The page communicates the property clearly and drives action.

- Replace placeholder meta tags (title, description, OG image) with real content
- Build single-page layout:
  - Hero section (name, tagline, hero photo)
  - Property overview (3 bed, 6 guests, Swaledale setting — sourced from AirBnB listing)
  - Photo gallery or image grid
  - Key features / highlights section
  - WhatsApp CTA (prominent, mobile-friendly)
  - AirBnB link (secondary CTA)
  - Google Maps link (location)
  - Footer (minimal)

**Done when:** Page accurately represents the property and CTAs work end-to-end.

---

## Phase 3 – Launch & Validate

**Goal:** Site is publicly live on the correct domain and discoverable.

- Point `garthgunnerside.co.uk` DNS to Vercel
- Verify HTTPS is active
- Submit sitemap to Google Search Console
- Manually verify WhatsApp and AirBnB links on mobile
- Smoke test page load speed (Vercel analytics or Lighthouse)

**Done when:** Domain resolves, Google Search Console is receiving data, and all links are confirmed working.

---

## Risks & Unknowns

| Risk | Likelihood | Mitigation |
|---|---|---|
| SEO ranking takes months for a new domain | High | Expected — not a launch blocker |
| Client-supplied photos are low quality | Medium | Use AirBnB listing photos as fallback initially |
| WhatsApp link behaviour varies by device | Low | Test on iOS and Android before launch |
| AirBnB listing photos may have usage restrictions | Medium | Confirm with client; use only photos they own |
