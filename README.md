# QuestiQ — Question Everything

Landing page for **QuestiQ**, a community-driven token on Solana.

Single-file static site — pure HTML/CSS/JS, no build step, no dependencies.

## Deploy on GitHub Pages

1. Create a new repository (e.g. `questiq-site`)
2. Upload everything in this folder to the repo root
3. Go to **Settings → Pages**
4. Under **Build and deployment**, set Source to **Deploy from a branch**, choose **main** and **/ (root)**, then Save
5. The site goes live in about a minute at `https://YOUR-USERNAME.github.io/questiq-site/`

### Custom domain (optional)

1. In **Settings → Pages → Custom domain**, enter your domain and save (GitHub creates a `CNAME` file automatically)
2. At your DNS provider:
   - **Subdomain** (e.g. `www.`): add a CNAME record pointing to `YOUR-USERNAME.github.io`
   - **Apex domain** (e.g. `questtoken.com`): add A records pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. Check **Enforce HTTPS** once the certificate is issued (can take a few minutes)

## Pre-launch checklist

Search `index.html` for **TODO** — every placeholder is tagged:

- [ ] Buy buttons → live FOMO launch link (hero + CTA section)
- [ ] "Buy on Pump.fun" button in the hero → Pump.fun coin link
- [ ] Footer social links: X, Telegram, Discord, GitHub
- [ ] `og:url` → your live URL
- [ ] `og:image` / `twitter:image` → `https://YOUR-LIVE-URL/og-image.png` (a placeholder image is included in this repo — replace it with branded art anytime)
- [ ] Optional: swap the SVG emblem in the hero for your real `logo.png`

## Files

| File | Purpose |
|---|---|
| `index.html` | The entire site — markup, styles, and scripts in one file |
| `og-image.png` | 1200×630 social share preview image (placeholder) |
| `robots.txt` | Allows search engines to index the site |
| `.nojekyll` | Tells GitHub Pages to skip Jekyll processing |
| `.gitignore` | Keeps OS junk files out of the repo |

## Local preview

Open `index.html` directly in a browser, or serve it:

```
python3 -m http.server 8000
```

then visit `http://localhost:8000`
