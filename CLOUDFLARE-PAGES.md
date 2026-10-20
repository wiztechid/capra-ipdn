# CAPRA IPDN — Cloudflare Pages (production)

- Hosting: Cloudflare Pages project `capra-ipdn`, URL `https://capra-ipdn.pages.dev/`
- Source: `wiztechid/capra-ipdn` `main`, static root output `.` and no build step
- Old URL: `https://wiztechid.github.io/capra-ipdn/` remains online temporarily for transition
- SEO: page canonical, Open Graph, structured data, robots.txt, sitemap.xml target the Pages hostname
- Deploy method: Cloudflare Pages API `POST /accounts/{account_id}/pages/projects/capra-ipdn/deployments` with multipart `branch=main` and `commit_hash=<sha>` (Git automatic event may require reconnect)
- Migration gate: test homepage, four articles, bot privacy page, assets, sitemap, links, and legacy URL before announcing URL change
- Avoid enabling ads until publisher approval and review of privacy, consent, and ad creative safety.

Legacy GitHub Pages links use a conditional JavaScript `location.replace` redirect by host/path, because github.io cannot serve configurable HTTP 301 redirects. This is a fallback supported by Google, though less robust than server 301. Preserve the old site and do not disable GitHub Pages until indexing and traffic transitions.
