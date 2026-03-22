# Technical Decisions

## 1. Framework

| | |
|---|---|
| **Options** | Plain HTML/CSS, Next.js, Astro, Vite + React |
| **Tradeoffs** | Plain HTML is simplest but lacks SEO tooling and component structure. Next.js is familiar on Vercel but overkill for a static page. Astro is purpose-built for static, content-focused sites with excellent SEO defaults and zero JS by default. |
| **Recommendation** | **Astro** — optimal for a static, SEO-first single-page site. Ships no JS by default, fast to build, and deploys to Vercel trivially. |
| **Risks** | Less familiar than Next.js, but minimal learning curve for a single page. |
| **Deferred** | If content grows or a blog is needed, Astro supports that without migration. |

---

## 2. Hosting & Deployment

| | |
|---|---|
| **Options** | Vercel, Netlify, GitHub Pages |
| **Tradeoffs** | All are free for static sites. Vercel has the best Astro integration and is already familiar to the developer. |
| **Recommendation** | **Vercel free tier** — zero config deployment from a GitHub repo. |
| **Risks** | None material for this use case. |
| **Deferred** | Custom domain DNS configuration (`thegarthgunnerside.co.uk`) to be done at deploy time. |

---

## 3. Styling

| | |
|---|---|
| **Options** | Tailwind CSS only, Tailwind + DaisyUI, plain CSS |
| **Tradeoffs** | Plain CSS is slowest to build with. Tailwind alone is flexible but requires hand-crafting all UI patterns. DaisyUI adds a component layer on top of Tailwind — pre-built, themeable components (buttons, cards, heroes) that significantly speed up UI development with no extra runtime cost. |
| **Recommendation** | **Tailwind CSS + DaisyUI** — accelerates UI development, looks polished out of the box, and adds no JS overhead. |
| **Risks** | DaisyUI's default themes may need overriding to achieve the right aesthetic for a rural holiday let. |
| **Deferred** | Theme selection (e.g. a warm, natural palette) to be decided during build. |

---

## 4. SEO Strategy

| | |
|---|---|
| **Options** | Manual meta tags only, structured data (JSON-LD), third-party SEO tools |
| **Tradeoffs** | Manual meta tags are necessary baseline. JSON-LD structured data (LodgingBusiness schema) meaningfully improves Google's understanding of the property with minimal effort. Third-party tools are unnecessary. |
| **Recommendation** | **Manual meta tags + JSON-LD structured data** — covers all meaningful SEO fundamentals without complexity. |
| **Risks** | New domain will take time to build authority. SEO success is not purely technical — content quality and backlinks matter. |
| **Deferred** | Google Search Console verification — done post-launch. |

---

## 5. Content Management

| | |
|---|---|
| **Options** | Hardcoded in source, headless CMS (e.g. Sanity), markdown files |
| **Tradeoffs** | A CMS adds infrastructure and maintenance overhead for a single page of content that rarely changes. Hardcoded is simplest and appropriate. |
| **Recommendation** | **Hardcoded in source** — developer maintains content via code. |
| **Risks** | If the client ever wants to self-manage content, a CMS would be needed. Assessed as low risk given the maintenance model. |
| **Deferred** | — |
