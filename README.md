# FinCalGlobal

Free financial calculators for loans, savings, retirement, tax, everyday money and business, plus dashboards and custom calculators for businesses: https://fincalglobal.com

The site is static HTML, so it runs on GitHub Pages with no build step. Every calculator has its own page and address, such as `/emi-calculator/`, so search engines can index and rank each one separately.

## What's in the repository

| Path | Purpose |
| --- | --- |
| `index.html` | Home page |
| `<calculator>/index.html` | One page per calculator (57 pages), plus `services/`, `privacy-policy/` and `contact/` |
| `og/*.png` | A social sharing image for every page |
| `favicon.svg`, `favicon.ico`, `favicon-32.png`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `site.webmanifest` | Browser, phone and app icons |
| `sitemap.xml`, `robots.txt` | Tell search engines which pages to crawl |
| `CNAME` | Serves the site at fincalglobal.com |
| `.nojekyll` | Publishes the files exactly as they are |
| `404.html` | Sends broken links back to the home page |

## Publish on GitHub Pages

1. Upload everything in this folder to the root of your repository, including the hidden `.nojekyll` file, and replace the old files.
2. **Settings › Pages**: Source **Deploy from a branch**, branch **main**, folder **/ (root)**.
3. Custom domain **fincalglobal.com**, then **Enforce HTTPS** once the DNS check passes.

DNS records (check GitHub's current guide: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site):

| Type | Host | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153 (one record each) |
| AAAA | @ | 2606:50c0:8000::153, 2606:50c0:8001::153, 2606:50c0:8002::153, 2606:50c0:8003::153 |
| CNAME | www | YOUR-USERNAME.github.io |

## After the site is live

1. **Google Search Console** (https://search.google.com/search-console): add `fincalglobal.com` as a Domain property, verify it with the DNS TXT record it gives you, then submit `https://fincalglobal.com/sitemap.xml` under **Sitemaps**.
2. **Bing Webmaster Tools** (https://www.bing.com/webmasters): import the site from Search Console.
3. Test pages with Google's **Rich Results Test** (https://search.google.com/test/rich-results) and **PageSpeed Insights** (https://pagespeed.web.dev).
4. When you add a YouTube video to a page, update its upload date in the page's structured data.
