# penumbraspace.com

Static website for Penumbra Autonomy. Plain HTML and images, no build step.

| File | Page |
|---|---|
| `index.html` | Home: hero, capabilities, problem, applications, team, contact |
| `applications.html` | Applications |
| `team.html` | Team |
| `assets/` | Logo, favicon, photos, images |
| `CNAME` | Custom domain for GitHub Pages (`penumbraspace.com`) |

## Deploy (GitHub Pages)
Settings → Pages → Source: **Deploy from a branch** → Branch: `main`, folder `/ (root)` → Save.
Custom domain: `penumbraspace.com` (already set by the `CNAME` file), then tick **Enforce HTTPS** once the certificate is issued.

DNS at the domain registrar:
- `A` records for `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
- `AAAA` records for `@` (optional): 2606:50c0:8000::153, 2606:50c0:8001::153, 2606:50c0:8002::153, 2606:50c0:8003::153
- `CNAME` record for `www`: `<org-name>.github.io`

Leave the existing `MX` / email records untouched.

## Editing
Edit the HTML directly; styles are included in each page. Accent color: `#FFC000`. The homepage uses Manrope with JetBrains Mono labels; the other pages use Julius Sans One headings and Didact Gothic body text. Fonts are loaded from Google Fonts.
