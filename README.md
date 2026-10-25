# Wander Wave Tours — SEO, GEO & AEO upgrade

This package updates the earlier **live static landing-page version** of Wander Wave. The professional booking/backend project from other versions is NOT included here. No Resend/Google Sheets variables are modified.

## Changes
- Updated visible New Cairo office address to the public Google Maps business listing; both map buttons use the matching Google Maps place ID.
- Kept the same logo artwork and site design, moving duplicate inline logo images into one local asset to reduce the HTML payload.
- SEO: unique homepage title, compelling description, canonical, robots, sitemap, Open Graph, X/Twitter preview, semantic heading content.
- GEO: `TravelAgency`, `WebSite`, `WebPage` and `FAQPage` JSON-LD showing business identity, contact, address and source social pages. GEO here means Generative Engine Optimization.
- AEO: visible FAQs with matching schema answers. Google does not generally display FAQ rich results for travel-company websites.
- Removed unsupported example testimonials generated during the original prototype and replaced them with verifiable service information and a Google Maps reviews link.
- Preserved WhatsApp leads to +20 10 70752150, other CTAs and the original design.

## Deployment to the current Vercel domain
1. Back up the existing Git repository/project. Confirm that the deployed site is this static version before replacing anything.
2. Copy **the contents of this folder** (`index.html`, `assets/`, `robots.txt`, `sitemap.xml`) into the root of that repository or deploy via Vercel CLI from this folder.
3. If using GitHub integration, commit and push; Vercel redeploys automatically. If using CLI: `vercel --prod` (after linking the correct project).
4. Do NOT replace a newer live Next.js site or booking backend with this static package; if your live project is different, apply these changes to its source files instead.
5. After deployment, open `/robots.txt`, `/sitemap.xml` and the page to verify.
6. In Google Search Console, submit sitemap and request indexing for the homepage.
7. Recheck/confirm the latest Maps address and office hours in your Google Business Profile and the site's location section.

## Assumptions requiring a business-owner check
- Public Maps listing captured: `2FX7+HPV, El Sheikh Abdel Gelil Eissa Street, New Cairo 1, Cairo Governorate 11835, Egypt`.
- No office hours marked up because the booking window described as 09:00–21:00 differs from public Google Maps business hours shown as 10:00–22:00; add opening hours only once confirmed.
- SEO/GEO/AEO cannot guarantee particular search or AI results.

## Checks
- Google Rich Results Test: https://search.google.com/test/rich-results
- Schema validator: https://validator.schema.org/
- Google Search Console: https://search.google.com/search-console
