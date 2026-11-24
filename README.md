# FinCalGlobal

Free financial calculators for loans, savings, retirement, tax, everyday money and business: https://fincalglobal.com

The whole site is one static page (`index.html`), so it runs on GitHub Pages with no build step.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The website: all calculators, the privacy policy and the contact page |
| `CNAME` | Tells GitHub Pages to serve the site at fincalglobal.com |
| `.nojekyll` | Serves the files as they are, without Jekyll processing |
| `404.html` | Sends broken links back to the home page |
| `favicon.svg`, `apple-touch-icon.png` | Browser tab and phone home-screen icons |
| `og-image.png` | Preview image when the site is shared on social media |
| `robots.txt`, `sitemap.xml` | Help search engines find and index the site |

## Publish on GitHub Pages

1. Create a new **public** repository on GitHub, for example `fincalglobal`.
2. Upload every file in this folder to the root of the repository, including `.nojekyll` (it's hidden on some computers).
3. In the repository, open **Settings › Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose **main** and **/ (root)**, then **Save**.
5. Under **Custom domain**, confirm it shows `fincalglobal.com` (the `CNAME` file sets it).
6. When the DNS check passes, tick **Enforce HTTPS**.

## DNS records at your domain registrar

Replace `YOUR-USERNAME` with your GitHub username.

| Type | Name / host | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| AAAA | @ | 2606:50c0:8000::153 |
| AAAA | @ | 2606:50c0:8001::153 |
| AAAA | @ | 2606:50c0:8002::153 |
| AAAA | @ | 2606:50c0:8003::153 |
| CNAME | www | YOUR-USERNAME.github.io |

DNS changes can take up to 24 hours. Check GitHub's current guide before you start: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

## Updating the site

Edit `index.html` (or upload a new version) and commit. GitHub Pages republishes within a minute or two.

## Contact

support@fincalglobal.com
