# ZITO Equine — project brief for Claude Code

## What this is
Marketing website for ZITO Equine, a stallion owner. Project comes through
Chelsea Shaffer (Equine Network side work). Built and maintained by
Kari DeCastro / Idlewild Creative LLC — the client does NOT edit the site.

## Stack
- Plain static HTML / CSS / vanilla JS. No build step, no framework.
- Hosted on Netlify, auto-deploys on push to `main`.
- Repo lives in the `idlewild-creative` GitHub org.
- Forms use Netlify Forms (`data-netlify="true"`), no backend.

## Structure
- `index.html` — home
- `stallions/` — one page per stallion (copy `stallions/_template.html`)
- `breeding.html` — breeding info, fees, shipping, contracts
- `contact.html` — breeding inquiry form (Netlify Forms)
- `css/style.css` — all styles; design tokens live at the top in `:root`
- `js/main.js` — mobile nav + small enhancements only
- `images/` — site images; `images/stallions/` for stallion photos

## Conventions
- Keep header/footer markup identical across pages (no includes — edit all pages).
- Mobile-first, must look good at phone width.
- Compress images before committing (aim < 300 KB each, use .webp or .jpg).
- Every page needs a unique <title> and meta description.
- Explain changes to Kari in plain English, not jargon.

## Deploy
    git add -A
    git commit -m "describe the change"
    git push

## Still to gather from client
Logo, brand colors, stallion names + pedigrees + photos/video, stud fees,
breeding terms, contact info, domain + where DNS lives.
