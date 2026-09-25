# ZITO Equine — project brief for Claude Code

## What this is
Marketing website for ZITO Equine, owned by David Zito. Project comes through
Chelsea Shaffer (Equine Network side work). Built and maintained by
Kari DeCastro / Idlewild Creative LLC — the client does NOT edit the site.

The operation is bigger than the two flagship stallions currently on the site
(Dirty Fling, WSR Hesa Dunofa Lena "Rooster"). There are additional unproven
stallions (may or may not be featured), a band of mares (some to be
highlighted), and locations in Colorado and Arizona in addition to where the
stallions stand at stud (Solo Select in TX, Lazy E in OK). David Zito also
competes himself, with success at the Riata. Don't assume the current
2-stallion, 2-location scope is the full picture when planning site structure.

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
- Domain + where DNS lives.
- Photo for WSR Hesa Dunofa Lena "Rooster" (Dirty Fling's photo is in).
- Decision on which additional (unproven) stallions to feature, if any.
- Mare band info + photos, and which mares to highlight.
- Details on the Colorado and Arizona locations (what happens at each).
- David Zito's own competition bio/results (Riata success) — likely an About page.
- Media page content (press, video, etc. — scope still undefined).
- A family photo — Kari needs to shoot this in person at the Arizona property.
- Foal photos for a future foal gallery (probably wanted, no photos yet).
