# On-Page SEO Checklist

Canonical on-page SEO reference shared by every content-generation skill (vShopper blog, BIS blog, BIS service pages). Every page-generation skill reads this file before generating any page. Every page shipped must satisfy every applicable item below. Technical SEO (sitemaps, robots.txt, Core Web Vitals) and off-page SEO (backlinks, citations) are handled separately — this file is on-page only.

---

## HEAD / METADATA

- [ ] **Title tag**: 50–60 chars, primary keyword near the start
- [ ] **Meta description**: 150–160 chars, primary keyword + benefit + soft CTA
- [ ] **Canonical URL** set to prevent duplicates
- [ ] **Open Graph tags**: `og:title`, `og:description`, `og:image` (1200×630), `og:url`, `og:type`
- [ ] **Twitter Card tags**: `twitter:card=summary_large_image`, `twitter:title`, `twitter:description`, `twitter:image`
- [ ] **Language attribute** on `<html>` (`lang="en"`)
- [ ] **Viewport meta tag**
- [ ] **Favicon** + `apple-touch-icon`
- [ ] **Charset meta** (`utf-8`)

## URL STRUCTURE

- [ ] **Short slug** (under 60 chars)
- [ ] **Primary keyword** in the slug
- [ ] **Hyphens** only — never underscores
- [ ] **Lowercase** only
- [ ] **No stop words** ("the", "a", "of") unless necessary for clarity
- [ ] **Logical hierarchy**: `/services/[service-name]`, `/blog/[post-slug]` (BIS) or `/blogs/[handle]/[post-slug]` (vShopper/Shopify)

## HEADINGS

- [ ] **Exactly one H1** per page, contains primary keyword
- [ ] **Logical H2 → H3** hierarchy (never skip levels)
- [ ] **H2s** use supporting keywords + questions from the cluster
- [ ] **No keyword stuffing** — write naturally

## COPY / BODY

- [ ] **Primary keyword** in the first 100 words
- [ ] **Direct answer** to the query in the first paragraph
- [ ] **Length** matches SERP average (within 20% of top-3 word count)
- [ ] **Short paragraphs** (1–4 sentences)
- [ ] **Readability**: 8th–10th grade level
- [ ] **Active voice** preferred
- [ ] **Bold key phrases** (sparingly)
- [ ] **Bullets and numbered lists** where appropriate

## FAQ SECTION (every blog post)

- [ ] **4–8 questions** from Ahrefs' "Questions" view (or People Also Ask) for the primary keyword
- [ ] **Direct, clear answers** (2–4 sentences each)
- [ ] **FAQ schema** (JSON-LD) applied

## IMAGES

- [ ] **Alt text** describes the image + keyword where natural
- [ ] **Descriptive filenames** with hyphens (e.g. `fibre-installation-sandton.webp`)
- [ ] **WebP format**, compressed under 200 KB
- [ ] **Width/height attributes** specified (prevents CLS)
- [ ] **Lazy loading** (`loading="lazy"`) for below-fold images
- [ ] **Responsive srcset** where needed
- [ ] **Featured/hero image** for social sharing

## INTERNAL LINKS

- [ ] **3–5 internal links** per post
- [ ] Link to **related blog posts** and **relevant service/product pages** — every linked URL verified to actually exist before linking, never invented
- [ ] **Descriptive anchor text** — never "click here" or "read more"
- [ ] **Contextually placed** in body copy
- [ ] **Breadcrumb navigation** on every page

## EXTERNAL LINKS

- [ ] **2–3 external links** to authoritative sources (.gov, .edu, major industry sites — ICASA, Vodacom, .ac.za sources are good fits for either brand)
- [ ] **Relevant** to the topic
- [ ] Open in **new tab** with `rel="noopener"`
- [ ] `rel="nofollow"` for sponsored links

## SCHEMA MARKUP (JSON-LD)

- [ ] **Article** schema on blog posts
- [ ] **LocalBusiness** schema on homepage, about, contact (BIS: `LocalBusiness` or more specific subtype; vShopper: `LocalBusiness` per store location)
- [ ] **Service** schema on BIS service pages
- [ ] **FAQ** schema wherever an FAQ section exists
- [ ] **BreadcrumbList** schema on every page
- [ ] **Organization** schema (site-wide)
- [ ] **Author/Person** schema for author bylines

## E-E-A-T SIGNALS

- [ ] **Author byline** with name on every blog post
- [ ] **Author bio** with credentials (years experience, role)
- [ ] Link to **author's dedicated page**, if one exists
- [ ] **Published date** displayed
- [ ] **"Last updated" date** when content is refreshed
- [ ] **Real stories, real numbers, real opinions** — pulled from the brand's `references/` files, never invented facts presented as verified
- [ ] **Cite authoritative sources**
- [ ] **About page** with full company credentials
- [ ] **Contact page** with real address, phone, business hours

## ACCESSIBILITY (affects SEO)

- [ ] **Semantic HTML5** tags: `<header>`, `<nav>`, `<main>`, `<article>`, `<aside>`, `<footer>`
- [ ] **ARIA labels** on interactive elements where needed
- [ ] **Color contrast** meets WCAG AA (4.5:1 for body text)
- [ ] **Focus indicators** visible on all interactive elements
- [ ] **Alt text** on ALL images (empty `alt=""` for decorative only)
- [ ] **Descriptive link text**
- [ ] **Skip-to-content** link for keyboard users

## MOBILE / RESPONSIVE

- [ ] **Responsive layout**
- [ ] **Touch targets** minimum 48×48 px
- [ ] **Body font size** minimum 16 px
- [ ] **No horizontal scroll** at any viewport
- [ ] **No intrusive interstitials**

## SOCIAL PREVIEW

- [ ] **Open Graph image** optimized (1200×630, under 1 MB)
- [ ] **Twitter Card image** (1200×600)
- [ ] **Compelling `og:description`** (different from meta if valuable)

## CONVERSION ELEMENTS (BIS service pages only — not blog posts, not vShopper)

- [ ] **Primary CTA** above the fold ("Request a callback" per BIS voice rules — never "book a consultation")
- [ ] **Phone number** with click-to-call (`tel:`)
- [ ] **Multiple CTA placements** throughout the page
- [ ] **Trust signals**: certifications, response-time commitments, years in business
- [ ] **Testimonials with names**, only if real — see `bis/references/stories.md`
- [ ] **Service-area coverage** listed
- [ ] **Business hours** displayed
- [ ] **Physical address** with embedded map, if applicable

## LONG-FORM CONTENT (1500+ words)

- [ ] **Table of contents** with anchor links at the top
- [ ] **Jump links** for each H2 section
- [ ] **Back-to-top** button

---

## How to use this file

1. Every page-generation skill reads this file before generating any page.
2. Every page must satisfy every applicable item — no exceptions.
3. **Conversion Elements** apply to BIS service pages only.
4. **Long-Form Content** items apply to any post 1500+ words.
5. vShopper runs on Shopify — some items (canonical, OG tags, schema, sitemap) are partly handled by the platform already and topped up by the existing "Biweekly SEO Maintenance" scheduled task. This checklist still applies in full to the content itself (headings, copy, FAQ, internal/external links, images).
