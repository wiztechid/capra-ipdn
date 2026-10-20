# CAPRA IPDN — Publisher Readiness & Ad Safety SOP
Updated: 2026-10-20

## Production baseline
- URL: https://capra-ipdn.pages.dev/
- Source: wiztechid/capra-ipdn (main), deployed automatically to Cloudflare Pages.
- Publisher: NOT submitted; NOT approved; NO ad scripts installed at time of audit.
- Public trust pages: about, contact, privacy, privacy-bot, disclaimer, terms.
- Sitemap contains 14 canonical Cloudflare Pages URLs after the 2026-10-20 post-SKD update.
- All pages identify CAPRA IPDN as an independent community website, not an official IPDN or government service.

## Publisher application quality gate
1. Verify HTTPS homepage, all articles, legal pages, sitemap and robots.
2. Verify eligibility of Cloudflare Pages free subdomain in Adsterra dashboard; acceptance is not guaranteed.
3. Confirm all visible buttons work and no incomplete tool is advertised as live.
4. Verify factual selection dates against current official SPCP/BKN documents before changing editorial dates.
5. Revise privacy and consent disclosures before introducing ad scripts or new analytics.
6. Submit exact public URL and request appropriate display/native format; no claim of approval before provider confirmation.

## Ad safety & UX policy
- Use at most one modest banner in the first pilot, clearly labeled Iklan.
- Never obstruct official PDF links, maps, exam guidance, rankings, or primary navigation buttons.
- Avoid Popunder, OnClick, masked Smartlinks, Social Bar, misleading notifications and fake download buttons.
- Keep BOOST CPM OFF; request campaign exclusions for adult, gambling, deceptive finance, fake government announcements, and fake examination guarantees.
- No artificial, paid incentivized, bot, or click-exchange traffic.
- If unsuitable ad creative appears, suspend the placement and request campaign blocking.
- Do not install any ad script until the account, site and ad unit are approved and user authorizes installation.

## Regression checks
- Test 375px, 768px, and 1440px layouts for horizontal scrolling, navigation and cards.
- Inspect province search and passing-grade interactive data after every functional change.
- Check all share links direct to capra-ipdn.pages.dev (not previous github.io).
- Check sitemap, canonical URLs, OG references, robots and Google Search Console independently.
- Keep old GitHub Pages JavaScript redirect so existing shared links retain their destination.
- Do not interpret hosting or sitemap success as proof of Google indexing or Adsterra approval.

## Reporting / rollback
- Public issues: https://github.com/wiztechid/capra-ipdn/issues
- Community: https://t.me/capraipdn
- Never collect NIK, OTP, passwords, card information or individual exam records through public channels.
- Roll back Cloudflare Pages to the last successful deployment; revert commits instead of rewriting Git history.

## Editorial change log — 20 October 2026
- Fixed inaccurate SKD date (22–29 September, not through 29 October) and homepage stage logic.
- New user-intent gaps: official stage-I health results per 38 provincial annexes, psychology/gladi preparation, consolidated selection-later schedule and final selection.
- Editorial source: SPCP IPDN 2026 official announcement pages. Do not copy personal candidate data into our server.
- Official SPCP homepage and selection-later schedule have conflicting final-selection regional dates; article documents discrepancy and defers to the newest official notice.
- Keyword potential is qualitative based on timely user intent; no independently verified search-volume or SERP competition metric was obtained. Do not invent monthly volume.
- Source PDF for psychology was linked from SPCP but could not be independently extracted during this update. Article therefore does not assert detailed clothing, devices, exam-session rules.

## Article SEO publication gate — 20 Oct 2026
- Three post-SKD articles keep unique search intent and canonical slugs; do not duplicate existing URLs.
- Unique H1 and title/description; named source SPCP; author/publisher Article JSON-LD; Open Graph/Twitter large-image metadata.
- Three illustrated WebP hero assets (1672×941, roughly 215–264 KiB) are deployed at repository root: /hasil-tes-kesehatan-ipdn-2026.webp, /tes-psikologi-ipdn-2026.webp, /jadwal-seleksi-lanjutan-ipdn-2026.webp. Earlier SVG assets remain as unreferenced backup.
- Image is illustrative, not an official document or exam result. No personal data in images or article body.
- Recheck page live, article date, dynamic site timeline and official announcements before claiming freshness; verify mobile when supported.

## Homepage featured articles QC — 20 Oct 2026
- The three newest post-SKD articles are visible as image-led linked feature cards in a single primary homepage section: results, psychology, and selection-later schedule.
- Each featured card uses its corresponding published WebP image, descriptive alt text, unique H3, source/date label, summary, and direct canonical internal URL.
- Older SKD cards remain indexed and linked but are explicitly titled ARSIP SKD; any prior unverified most-popular claims are removed.
- Verified 20 Oct 2026: creative WebP images are installed on article pages and the homepage. Do not mistake an illustrative image for an official document or official IPDN portrait.
- Desktop grids are 3-column, tablet 2-column, narrow mobile 1-column; visually verify after deployment.

## Unified article homepage policy — 20 October 2026
- Exactly one unified section `#artikel-utama` lists recent and earlier article content in the same card design (consistent thumbnail, title, date, category, CTA).
- Maximum 9 article cards on homepage, newest publication date first (not date of event/announcement and not cosmetic template updates).
- Article source manifest: `article-index.json`, with distinct slug, published date, hero thumbnail, description, and category. Keep static HTML cards synchronized on publishing or updating articles; preserve crawlable HTML instead of JS-only rendering.
- Present article labels for SKD as archive within the same grid rather than in a separate article section.
- Structured data: an ItemList records the identical published order for the visible cards.
- Existing individual article URLs, source references and canonical are unchanged. New article requires a new unique slug and a homepage refresh based on the manifest (latest 9 only).
- Homepage navigation points to `#artikel-utama`; the former `#info-terbaru` anchor remains as a hidden compatibility anchor for old internal/external links.

## 2026-10-20 WebP image rollout
- Replaced SVG display images in three October articles and three featured homepage cards with the uploaded WebP assets. Did not modify article slugs, article count (7), order (newest first), legacy GitHub Pages redirects, or sitemap URLs.
- Kept fallback SVG assets in git for safe rollback. Corrected social preview image URLs and dimensions and Article JSON-LD ImageObject fields.
- Visual publication must be verified on production after Cloudflare Pages GitHub push finishes; browser cache may require a hard refresh.
