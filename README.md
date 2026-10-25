# Lumos Dental & Aesthetic Clinic: SEO, AEO and GEO

AiS LABZ engagement workspace for **lumosclinics.com**. The site is built on WordPress, Elementor, Rank Math and LatePoint, and is hosted on Hostinger. The clinic is at Unit 3501, Aspin Commercial Tower, Sheikh Zayed Road, Dubai.

The engagement started on 25 October 2026. Scope and roadmap follow the AiS LABZ proposal dated 21 October 2026: a six-month programme covering SEO, AEO, GEO, the Google Business Profile, and UI/UX guidance.

Open **`index.html`** in a browser for the full baseline audit dashboard.

## Baseline (25 Oct 2026)

24 findings across all 127 HTML pages: 7 critical, 9 high, 8 medium. All of the proposal's audit figures were reproduced exactly. Six of the findings are new and were not in the proposal.

| Metric | Value |
|---|---|
| Pages crawled | 127 HTML pages (all HTTP 200) plus 1 KML file |
| Pages with `nosnippet`, including all 5 category hubs | 36 |
| Non-brand AI or search queries that cite Lumos | 0 of 10 |
| GPTBot access | HTTP 429, blocked at the CDN |
| Pages with exactly one H1 | 70 of 127 |
| Treatments published at two URLs | 16 pairs, plus 6 overlapping pages |
| Medical schema (MedicalClinic, Dentist, Physician, FAQPage) | 0 pages |
| Pages with a meta description | 98 of 127 |
| Titles over 60 characters | 80 |
| Images with no alt text | 1,891 |
| Mobile Lighthouse score | 29 (desktop 65) |
| Mobile LCP | 10.0 s (target 2.5 s or less) |
| Homepage weight | 14.4 MB, of which 7.6 MB is two hero videos |
| Server response time | 1.8–2.1 s, uncached |
| Phone numbers listed online for the clinic's unit | 4 (legacy "Fattan Polyclinic" listings) |

### New since the proposal

1. Old "Fattan Polyclinic" listings for the same unit (on DHR, Doctify, Edarabia and DRFive) carry conflicting NAP details.
2. The `<main>` element on the main dental and aesthetic hub pages is empty.
3. `/dentist-in-dubai/` shows lorem-ipsum copy and three "0 AED" prices.
4. Posts and category archives from the demo theme are still live.
5. `/survey-page/` links to a placeholder Google review URL, `YOUR_GOOGLE_REVIEW_LINK_HERE`.
6. The Salonist listing uses a hair-salon template.

## Repository layout

| Path | Contents |
|---|---|
| `index.html` | Baseline audit dashboard |
| `audit/crawl-2026-10-25.csv` | Data for each page: title, meta, robots, H1s, schema, images, word count, response time |
| `audit/lighthouse/` | Lighthouse summaries: homepage on mobile and desktop, and the veneers treatment template |
| `docs/ai-visibility-baseline.md` | AI-answer visibility, crawler access, NAP and entity findings, competitor set, citation targets |
| `docs/phase-1-plan.md` | Phase 1 changes, each with its location, evidence and effort |
| `docs/client-requests.md` | Access and information we need from Lumos |
| `implementation/redirects.csv` | 27 rules, 301 unless marked otherwise, in Rank Math import format |
| `implementation/schema-medicalclinic.jsonld` | Draft MedicalClinic + Dentist schema for the whole site; fields marked TBC need clinic input |
| `implementation/llms.txt` | Replacement llms.txt; fields marked TBC need clinic input |

## Status

### Phase 1: foundation and quick wins (weeks 1–4)

- [x] Baseline audit, which re-verifies the proposal's KPIs
- [x] AI visibility and competitor baseline
- [x] Redirect map, schema draft and llms.txt draft prepared
- [ ] Remove `nosnippet` from 36 pages
- [ ] Allow-list GPTBot on the Hostinger CDN
- [ ] Remove the lorem-ipsum text, "0 AED" prices, review-link placeholder and demo-theme posts
- [ ] Clean the sitemap: noindex the utility pages and add /about/
- [ ] Turn on full-page caching and replace the hero videos
- [ ] Set up Search Console, Bing Webmaster Tools and GA4 conversion tracking. *Blocked: Google access pending.*
- [ ] Audit the Google Business Profile and start the NAP clean-up. *Blocked: Google Business Profile access pending, and Lumos must confirm its relationship to Fattan.*
- [ ] Set the keyword baseline. *Blocked: Search Console access pending; Ahrefs and Semrush are unavailable on our current plans.*

## Method

- All sitemap URLs were fetched and parsed directly from the live site, so counts are measured, not estimated.
- Performance figures come from single Lighthouse 12.2.1 lab runs on headless Chromium. We have no field data.
- AI visibility is estimated from 13 patient-style web searches on a US-based search index. The proposal's monthly panel of 30 prompts, run across ChatGPT, Gemini, Perplexity and AI Overviews, replaces this estimate from Month 1.

Not yet covered:

- Keyword rankings and backlinks (Ahrefs: our plan does not include API access; Semrush: no API units left)
- Search Console, GA4 and Google Business Profile data
