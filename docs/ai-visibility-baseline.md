# AI visibility and competitive baseline, 25 October 2026

This is the starting position for the GEO and AEO workstreams (proposal sections 7 and 8).

## How this was measured

- We ran 13 searches written the way a patient would phrase a question to an AI assistant, and recorded which domains came up. The domains that rank for these searches are, in practice, the sources ChatGPT, Gemini and Perplexity draw on.
- The search index is US-based, so these results are only a rough proxy for what a searcher in the UAE sees.
- We fetched the site with each AI crawler's user agent.
- No paid tools were used. Ahrefs Brand Radar is not included in our current plan, and the Semrush account has no API units left.
- The proposal's monthly 30-prompt panel, run across ChatGPT, Gemini, Perplexity and AI Overviews, starts in Month 1 and replaces this proxy.

## Headline result

**Lumos did not appear in any of the 10 non-brand searches.**

- It appeared only for "dental and aesthetic clinic Sheikh Zayed Road", and only through a broken Salonist listing.
- Searches for the brand name return unrelated clinics with similar names (Lumara, Lumus, Lumiere, and a Malaysian "Lumos").

| Query | Lumos present? | Top domains cited |
|---|---|---|
| best dental clinic in Dubai | No | sothebysrealty.ae, propertyfinder.ae, gulfnews.com classifieds |
| best Hollywood smile clinic Dubai | No | aesthetics.kingscollegehospitaldubai.com, newswire.com |
| dental implants cost Dubai | No | zavis.ai (3 pricing pages), meddental.ae, lyfboat.com |
| best aesthetic clinic Dubai | No | graziamagazine.com/me, propertyfinder.ae, tradearabia.com |
| Profhilo Dubai price | No | emirateshospitals.ae, drfive.com, King's Aesthetics |
| exosomes treatment Dubai | No | emirateshospitals.ae, King's Aesthetics, luciaclinic.com |
| laser hair removal Dubai best clinic | No | doctify.com, bayut.com, King's Aesthetics |
| veneers Dubai price | No | meddental.ae, zavis.ai, bookimed.com, whatclinic.com |
| best dermatologist Jumeirah | No | doctify.com (all 10 results) |
| best cosmetic dentist Dubai 2026 | No | medicaltourism.com, emirateshospitals.ae, doctify.com |
| dental and aesthetic clinic Sheikh Zayed Road | Yes, through Salonist only | doctify.com, salonist.io, gulfnews.com |
| Lumos clinic Dubai (brand) | Directories only | salonist.io, zavis.ai, trustpilot (wrong brands) |
| Lumos clinic reviews (brand) | Weak | salonist.io, zavis.ai, magicpin (another "Lumos") |

## AI crawler access (measured on lumosclinics.com)

| Crawler | Response |
|---|---|
| GPTBot (OpenAI training) | **HTTP 429, blocked at the Hostinger CDN** |
| OAI-SearchBot, ChatGPT-User | 200 |
| ClaudeBot, PerplexityBot, Google-Extended, Googlebot, Bingbot, CCBot | 200 |

## Entity and NAP findings (new since the proposal)

**The clinic's unit has a previous occupant.** Unit 3501 in Aspin Tower is still listed online as **Fattan Dental & Derma Clinic / Fattan Polyclinic LLC**. Its listings are live on:

- the Dubai Health Regulator Waffer directory
- Doctify (0 reviews, wrong specialties)
- Edarabia
- DRFive
- Cureus

fattanclinic.com currently returns an SSL error (HTTP 526).

**Four phone numbers are in circulation** for this address:

- 04 352 4140 (Lumos)
- 04 355 0236, 056 997 8196 and 04 229 0018 (Fattan)

**Opening hours differ by listing:**

- Salonist: 8am–10pm
- Edarabia: 10am–9pm
- Doctify: 8am–8pm

**The brand name is not consistent:**

- On the website's own schema: "Lumos Polyclinic llc."
- In the WebSite schema: "Lumos Dental & Aesthetic Clinic in Dubai"
- On directories: "Lumos Polyclinic L.L.C"

**The Google profile appears healthy.** Zavis reports a Google rating of 4.9 from 93 reviews and 26 insurers accepted (last updated 11 April 2026). We have not yet checked this against the Google Business Profile itself; access is pending.

**The Salonist listing is wrong.** It uses a hair-salon template, has no phone or website, and shows 0 reviews.

**Lumos was not found on** Doctify, Okadoc, Practo, WhatClinic, Fresha, Yelp, Tripadvisor, Wikidata, or any Time Out, What's On, Bayut or Property Finder listicle.

**Location targeting needs adjusting.** The clinic is in Trade Centre 1, not Jumeirah, so local targeting should use Sheikh Zayed Road, Trade Centre, DIFC, Downtown and Business Bay phrasing, as the proposal recommends.

## Competitors most often cited

| Clinic | Domain | Why it wins citations |
|---|---|---|
| Aesthetics by King's College Hospital | aesthetics.kingscollegehospitaldubai.com | Appeared in 6 of 13 queries; deep treatment and blog library; offers page; doctor pages; Arabic |
| Emirates Hospitals | emirateshospitals.ae | `/cost-packages/` pages with AED prices (e.g. Profhilo AED 999–1,299) |
| Dr. Michael's Dental | drmichaels.com | About 1,250 Google reviews at 4.9; about 380 blog posts; Arabic and Russian hreflang; about 40 doctor pages |
| Versailles Dental | versaillesdentalclinic.com | About 114 blog posts; Google profile lists services with prices |
| Lucia Clinic | luciaclinic.com | About 55 doctor pages; before-and-after section; cost guides |
| Biolite | biolitedubai.com | About 841 URLs; "cost in Dubai" pages; before-and-after section |
| Eden Aesthetics | edenaestheticsclinic.com | Thin website; wins almost entirely through third-party listicles |
| Dr Joy Dental | (403 to our fetcher) | Present on Bayut, Sotheby's and Property Finder lists |

**What this means for Lumos.** The sources AI assistants cite for this market are mainly:

1. aggregators (Doctify, Zavis, WhatClinic, Bookimed, DRFive)
2. lifestyle and property listicles (Property Finder, Bayut, Sotheby's, Grazia)
3. treatment pages that publish AED prices

Lumos has none of the three today.

## Citation targets, in priority order

1. **Google Business Profile:** one name, phone 04 352 4140, one set of hours, services listed with AED prices, review velocity.
2. **Doctify:** create a Lumos practice with doctor profiles, and claim or retire the Fattan profile.
3. **Zavis.ai:** claim the listing and get onto its implant and veneer pricing pages.
4. **DHR Waffer, DHA registry, Edarabia, DRFive:** correct the legal name, phone and website.
5. **Salonist:** fix the listing or remove it.
6. **Property Finder, Bayut, Sotheby's Journal and Grazia ME** best-clinic lists, through outreach and PR.
7. **WhatClinic, Bookimed, MedicalTourism.com:** veneers, Hollywood smile and dental tourism.
8. **Okadoc:** booking and reviews.
9. **InsuranceMarket.ae** clinic guides, which fit Lumos because it accepts 26 insurers.
10. **Apple Business Connect and Bing Places.** Bing data feeds ChatGPT search and Copilot.
