# Specification: Phase 2 – Core Content

**Status:** Execution  
**Created:** 2026-03-22  
**Modified:** 2026-03-22  

---

## Exec Summary

Build the real single-page site for The Garth — a 3-bedroom holiday cottage in Gunnerside, Swaledale. Replace the Phase 1 placeholder with a complete, content-rich page that communicates the property clearly and drives guests to enquire via WhatsApp. The lead USP is the property's unrivalled panoramic views up and down Swaledale — this should be front and centre in all copy and visual choices. All copy and photos are sourced from the AirBnB listing. Structured data (JSON-LD) is included for SEO.

---

## Scope

### In Scope
- Replace placeholder meta tags with real title, description, and OG tags
- Build the full single-page layout (sections listed in Tasks)
- Static image grid (no lightbox — deferred to follow-up)
- WhatsApp CTA linking to `https://wa.me/+447757250718`
- AirBnB link to `https://airbnb.co.uk/h/thegarth`
- Google Maps link to Gunnerside village (exact pin deferred — business approval pending)
- JSON-LD structured data (`LodgingBusiness` schema)
- All copy drafted from AirBnB listing content (placeholder quality — owner to review)
- DaisyUI theme: **`autumn`** — warm, earthy tones fitting a rural Yorkshire property

### Out of Scope
- Photo lightbox / carousel (follow-up action)
- Availability calendar or booking forms
- Custom domain / DNS (Phase 3)
- Google Search Console submission (Phase 3)
- Analytics setup (Phase 3)
- Any content the owner has not yet supplied (we use AirBnB content as-is)

### Constraints
- Photos sourced from AirBnB listing (owner has access to originals if needed)
- WhatsApp is the only direct contact method — no email or phone
- No JS frameworks — Astro components only, zero client-side JS unless strictly necessary
- Single page — no routing

---

## Uncertainties

| # | Uncertainty | Status | Notes |
|---|---|---|---|
| 1 | AirBnB listing photos — copyright / usage | Open | Owner believes they own originals; treat as approved for now |
| 2 | Exact Google Maps pin unavailable | Noted | Using Gunnerside village link until Google Business approval clears |
| 3 | Copy accuracy | Open | All copy is drafted from AirBnB listing; owner must review before Phase 3 |
| 4 | OG image | Open | No dedicated OG image asset available; will use the primary hero photo |

---

## Page Layout

Sections in order, top to bottom:

1. **Hero** — full-width image, property name ("The Garth"), tagline, primary WhatsApp CTA button
2. **Overview strip** — 3 key stats: 3 bedrooms · 6 guests · Swaledale, Yorkshire
3. **About** — 2–3 paragraph property description (sourced from AirBnB)
4. **Highlights** — icon + label grid of key features (e.g. countryside views, private parking, dog-friendly, wood burner)
5. **Gallery** — static responsive image grid (no lightbox)
6. **Reviews** — 2–3 guest review cards (sourced from AirBnB)
7. **Find Us** — short location description + Google Maps link button
8. **CTA banner** — WhatsApp CTA (primary) + AirBnB link (secondary)
9. **Footer** — property name, copyright year, AirBnB link

---

## Tasks

| # | Task | Status |
|---|---|---|
| 1 | Switch DaisyUI theme to `autumn` in `tailwind.config` | ✅ Complete |
| 2 | Update meta tags (title, description, OG) with real content | ✅ Complete |
| 3 | Add JSON-LD `LodgingBusiness` structured data to `Layout.astro` | ✅ Complete |
| 4 | Build Hero section | ✅ Complete |
| 5 | Build Overview strip | ✅ Complete |
| 6 | Build About section | ✅ Complete |
| 7 | Build Highlights section | ✅ Complete |
| 8 | Build Gallery (static image grid) | ✅ Complete |
| 9 | Build Reviews section | ✅ Complete |
| 10 | Build Find Us section | ✅ Complete |
| 11 | Build CTA banner | ✅ Complete |
| 12 | Build Footer | ✅ Complete |
| 13 | Verify all CTAs (WhatsApp, AirBnB, Maps) resolve correctly | ⏸️ To Do |
| 14 | Smoke test: mobile layout looks correct | ⏸️ To Do |
| 15 | Owner review of copy and photos | ⏸️ To Do |

---

## Follow-up Actions

- **Lightbox/carousel** for the photo gallery (deferred from Phase 2)
- **Exact Google Maps pin** once Google Business Profile approval clears
- **Owner copy review** — all AirBnB-sourced text to be signed off before Phase 3 launch
- **OG image** — create a dedicated 1200×630 crop of the hero photo for social sharing
- **Phase 3:** DNS, HTTPS, Google Search Console, final link smoke test on mobile
