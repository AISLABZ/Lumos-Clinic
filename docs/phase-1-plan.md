# Phase 1: foundation and quick wins (weeks 1–4)

This phase covers proposal section 16, Phase 1. Each item gives the exact change, where it is made, and the evidence from the 25 October baseline.

| # | Change | Where | Evidence | Effort | Needs |
|---|---|---|---|---|---|
| 1 | Remove `nosnippet, noarchive` from all indexable pages | Rank Math → Titles & Meta → Pages, then per-post Advanced tab (35 pages use one ordering, 1 uses another) | 36 pages, including /dentist-in-dubai/, /cosmetic-dentistry-in-dubai/, /aesthetic-treatments-in-dubai/, /anti-aging-treatments-in-dubai/, /dermatology-skin-care-in-dubai/ | 30 min | WP access |
| 2 | Allow-list GPTBot | Hostinger hPanel → Security / CDN bot protection | GPTBot gets HTTP 429; every other AI crawler gets 200 | 15 min | Hostinger |
| 3 | `noindex` and remove from sitemap: /my-account/, /customer-dashboard/, /latepoint/, /latepoint-booking/*, /survey-page/, /sitemap/, /locations.kml | Rank Math → per-page Advanced → Robots; Sitemap settings → exclude | Utility pages currently in sitemap | 20 min | WP access |
| 4 | Add /about/ to the sitemap | Rank Math → Sitemap → Pages (check it isn't excluded) | /about/ returns 200 but is absent from the sitemap | 5 min | WP access |
| 5 | Remove the lorem-ipsum and "Starting at 0 AED" blocks | Elementor: /dentist-in-dubai/ and /treatments/dental-treatments-dubai/ | Lorem ipsum on 2 pages; three "0 AED" prices on /dentist-in-dubai/ | 30 min | WP access, real prices |
| 6 | Replace the `YOUR_GOOGLE_REVIEW_LINK_HERE` placeholder | /survey-page/ | Broken link (404) | 5 min | Review link |
| 7 | Remove demo-theme posts and taxonomies (Mindset, News, Cases, Formats, Media, Style, Trend, etc.) | Posts → delete the 2020 demo posts; delete the empty categories | /shine-by-lumos/ shows template posts such as "App developers that are going to slow down in 2020" | 30 min | WP access |
| 8 | Turn on full-page caching | Hostinger → LiteSpeed Cache / hPanel cache; CDN currently reports `DYNAMIC` | TTFB 1.8–2.1s on every page tested | 1 hr | Hostinger |
| 9 | Replace the autoplay hero videos with a poster image | Homepage, Elementor | Media is 7.6 MB of the 14.4 MB homepage | 1–2 hrs | Developer |
| 10 | Replace llms.txt with `implementation/llms.txt` (after the TBC fields are filled) | Hostinger Tools plugin, or a static file | Current file leads with legal pages, contains HTML entities and misspells "Dermathology" | 15 min | Clinic info |
| 11 | Set up Search Console, Bing Webmaster Tools and GA4 conversions (call, WhatsApp, LatePoint) | Google / GTM | Search Console meta tag found on only 1 page; no conversion baseline | 2 hrs | Google access |
| 12 | Google Business Profile audit; begin NAP clean-up (Fattan listings, Salonist) | Google profile + directories | See `docs/ai-visibility-baseline.md` | 3 hrs | Google profile access |
| 13 | Set the keyword baseline for the 12 clusters | Search Console + Keyword Planner | Ahrefs and Semrush unavailable on current plans | 3 hrs | Search Console access |

## Phase 2 (Month 2), already prepared

- **Redirect map:** `implementation/redirects.csv` holds 27 rules. 17 root-level shells redirect to their full `/treatments/` pages, and 4 slug fixes cover the malformed `https-lumosclinics-com-…` slugs and "viginismus". Import through Rank Math → Redirections → Import. Rename post slugs **before** adding the slug-fix rules. Confirm against Search Console clicks before applying.
- **Site-wide schema:** `implementation/schema-medicalclinic.jsonld` is the MedicalClinic + Dentist graph. Fill the TBC fields, then add it through Rank Math → Schema → Custom, or a site-wide snippet.
- **Template fix:** 23 treatment pages carry 3 to 19 H1s because headings such as "Benefits", "Step 1" and related-treatment cards are tagged as H1. 34 pages have no H1. One fix to the Elementor treatment template corrects most of them.
- **Title suffix:** "- Lumos Dental & Aesthetic Clinic In Dubai" adds 40 characters to every title. Change the Rank Math global separator and suffix to "| Lumos Clinic Dubai". This fixes most of the 80 titles over 60 characters.
