# Specification: Phase 1 – Foundation

**Status:** Complete  
**Created:** 2026-03-22  
**Modified:** 2026-03-22  

---

## Exec Summary

Initialise the Astro + Tailwind CSS + DaisyUI project, push to the existing GitHub repo, connect to Vercel, and confirm a live deployment URL exists. The output is a placeholder page — not final content — but with the real project structure, meta tags (placeholder values), and deployment pipeline in place.

---

## Scope

### In Scope
- Initialise Astro project with Tailwind CSS and DaisyUI
- Placeholder `index.astro` page (site name, one-line description, no real content)
- Basic meta tags: title, description, Open Graph (placeholder values)
- Vercel deployment config (`vercel.json` if needed — removed from scope per review)
- Developer connects project to Vercel and confirms live URL (manual step)

### Out of Scope
- Any real content, photos, or copy (Phase 2)
- DNS / custom domain (Phase 3 — domain not yet purchased)
- Analytics, SEO structured data, sitemap (Phase 2/3)
- WhatsApp / AirBnB CTAs (Phase 2)

### Constraints
- Vercel free tier
- No CMS — content managed in code
- Repo already exists on GitHub; Vercel connection handled by developer

---

## Uncertainties

| # | Uncertainty | Status | Notes |
|---|---|---|---|
| 1 | DaisyUI theme choice | Low risk | Developer to select a warm/natural theme; client reviews in Phase 2 |
| 2 | Domain `garthgunnerside.co.uk` not yet purchased | Noted | Not a Phase 1 blocker; flagged for Phase 3 |

---

## Tasks

| # | Task | Status |
|---|---|---|
| 1 | Initialise Astro project with Tailwind CSS + DaisyUI | ✅ Complete |
| 2 | Create placeholder `index.astro` with site name and one-liner | ✅ Complete |
| 3 | Add meta tags (title, description, OG) with placeholder values | ✅ Complete |
| 4 | Developer: push to GitHub and connect repo to Vercel | ✅ Complete |
| 5 | Confirm live Vercel URL is accessible | ✅ Complete |

---

## Follow-up Actions

- **Phase 2:** Replace all placeholder meta tag values (title, description, OG image) with real content
- **Phase 2:** Add real content, photos, and CTAs
- **Phase 3:** Purchase `garthgunnerside.co.uk` and point DNS to Vercel
- **Phase 3:** Connect Vercel to custom domain and verify HTTPS
- **Housekeeping:** Add `.vscode/settings.json` + `extensions.json` and `.gitignore` rule to selectively commit only project-relevant VS Code config
