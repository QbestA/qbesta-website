# Qbesta Website — Roadmap & Status

Single-page marketing/campaign site for **Qbesta** (AI implementation, agentic AI,
workflow automation & software development for Australian SMEs).
Hosted on **GitHub Pages** (free, push-to-`main` deploys), custom domain **www.qbesta.com**.

- **Stack:** plain HTML + vendored Bootstrap 5 (`css/styles.css`) + dark-theme overrides (`css/qbesta.css`). No build step.
- **Primary conversion goal:** *Book a free discovery call* (Formspree form → `team@qbesta.com`).
- Design spec: see `docs/superpowers/specs/` / approved plan from the redesign session.

---

## ✅ Shipped

### Redesign — campaign landing page (2026-06-01)
- [x] Rewrote `index.html` as a conversion-focused single page for Australian SMEs
- [x] Modern **dark theme + gold (#ffc800)** accent in `css/qbesta.css` (Bootstrap left untouched)
- [x] Hero with single repeated CTA (*Book a free discovery call*) + trust strip
- [x] Pain/promise strip
- [x] 6 service cards: Agentic AI · Workflow automation · AI implementation · Software development · AI readiness & strategy · Responsible AI & security
- [x] Agentic-AI explainer (chatbot vs rules vs agent)
- [x] 6 industry use cases (trades, professional services, health, retail/hospitality, real estate, accounting)
- [x] 5-step "How we work" process + "no value, no fee" line
- [x] Why Qbesta / what-sets-us-apart lists
- [x] "Technologies we work with" logos (replaced misleading fake client logos)
- [x] Testimonials section built — **currently hidden** (placeholder content; re-enable when real quotes exist)
- [x] FAQ accordion (cost, timeline, data/privacy, "do we need AI?", vendor lock-in)
- [x] Final CTA band + restyled discovery-call contact form (Formspree, unchanged endpoint)
- [x] Footer with legal entity + ABN 63460852097
- [x] SEO: title, meta description, canonical, Open Graph/Twitter tags (→ www.qbesta.com)
- [x] Compressed hero/band images (1–2.5 MB → 240–470 KB); `.gitignore` excludes raw Pexels originals
- [x] Removed clutter: fake client logos, lorem-ipsum portfolio modals, backup HTML files, `v5.3.3.zip`, `.DS_Store`
- [x] Verified locally: desktop + mobile render, 0 console errors, 0 broken anchors, mobile menu works

---

## 🔜 Next up — required to fully "go live" as a campaign target

These need **owner input** (IDs, links, settings) — placeholders are already in the code.

- [ ] **Confirm GitHub Pages settings** — source = deploy from `main`; custom domain `www.qbesta.com`; **Enforce HTTPS** ticked. Confirm `qbesta.com` (apex) redirects to `www`.
- [ ] **Add analytics / ad tracking** — paste GA4 / Google Ads tag into the marked `<head>` placeholder in `index.html` (replace `G-XXXXXXX`).
- [ ] **Fire a conversion event on form submit** — add a `gtag('event', 'generate_lead' …)` call in the contact-form success handler so campaign conversions are measurable.
- [ ] **Discovery-call booking** — decide: keep Formspree form only, or add the **Calendly** inline embed (commented placeholder already in the contact section) for self-service booking.
- [ ] **Verify footer LinkedIn URL** — currently `linkedin.com/company/qbesta`; confirm it exists or update.

## 📋 Backlog — content & polish

- [ ] **Testimonials** — the "What clients say" section is currently **hidden** (`hidden` attribute on `#testimonials`). Add real client quotes (name, business, city), replace the placeholder cards, then remove `hidden` to re-enable.
- [ ] **Case studies / results** — add 1–3 short before/after outcomes with numbers (strong on competitor sites).
- [ ] **Pricing / engagement model** — optional section or FAQ expansion (transparent ranges build trust).
- [ ] **Privacy Policy & Terms pages** — add real pages and link from footer (dead links were removed).
- [ ] **Lighthouse pass** — confirm performance/SEO/accessibility scores; add `loading="lazy"` to any below-fold imagery, check colour contrast on dark theme.
- [ ] **Favicon / OG image** — verify the social-share preview image renders well; consider a branded OG image.
- [ ] **Remove unused `bootstrap-5.3.3/` folder** — site uses the vendored `css/styles.css` + CDN JS, so the extracted Bootstrap dir is dead weight.
- [ ] **Fix remote URL casing** (optional) — repo canonical path is now `QbestA/qbesta-website`.

## 💡 Future / if/when needed (deferred by design)

- [ ] **Insights / blog section** — considered and deferred in favour of a focused single landing page; revisit if SEO/content marketing becomes a priority.
- [ ] Multi-page expansion (separate Services / Industries / About pages) — only if content outgrows the single page.
- [ ] Additional industry pages tailored to specific ad campaigns (landing-page variants per audience).

---

## New requirements

> Add new asks here as they come up, then promote them into the sections above.

- _(none yet)_
