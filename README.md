# Cherrylyn M. Alcaraz — Executive Portfolio

Personal portfolio site for **Cherrylyn "ChiChay" M. Alcaraz**, founder and operator of eight registered Philippine businesses across transport, industrial supply, automotive upholstery, catering, vehicle rental, distribution, and business support.

Calabarzon, Philippines · Est. 2012

---

## Live site

| Environment | URL |
|---|---|
| Netlify | _add your URL here_ |
| GitHub Pages | _enable in Settings → Pages_ |

## What's in the site

| Section | Content |
|---|---|
| Hero | Positioning, availability status, headline metrics |
| Stop 01 · Portfolio | Eight operating entities with logos and live links |
| Stop 02 · What I Do | Operations, compliance, finance, systems |
| Stop 03 · Proof of Execution | Six self-built production systems with demo videos |
| Stop 04 · Toolbox | Current stack and what's being explored |
| Stop 05 · Capital Markets | PSE and FX activity, self-built trading journal app |
| Stop 06 · Work With Me | Consulting, advisory, and executive engagement models |
| Stop 07 · How I Work | Operating principles |
| Contact | Direct contact, downloadable resume |

## Repository structure

```
index.html                     Complete site — logos, portrait and resume
                               are embedded as base64, no external assets
video/
  cdsc-portal-demo.mp4         CDSC Client Portal demo
  cdsc-poster.jpg              Video thumbnail
Cherrylyn-Alcaraz-Resume.pdf   Standalone copy of the executive resume
_redirects                     Netlify SPA routing config
```

## Tech

Single-file static site. No build step, no dependencies, no framework.

- Semantic HTML5
- CSS custom properties, CSS Grid, Flexbox
- Vanilla JavaScript — IntersectionObserver for scroll reveal and animated counters
- Inline SVG for all icons and tool logos
- Base64-embedded images and PDF so the page is fully self-contained
- Fonts: Playfair Display, Inter, IBM Plex Mono (Google Fonts)
- Fully responsive; respects `prefers-reduced-motion`

## Adding a demo video

Open `index.html` and find `const DEMOS`. Each system has an entry:

```js
chemfleet: { title:"ChemFleet", sub:"Fleet operations platform", url:"" },
```

Add a link between the quotes:

| Source | Example |
|---|---|
| Local file | `"video/chemfleet-demo.mp4"` |
| YouTube | `"https://youtu.be/XXXXXXX"` |
| Loom | `"https://www.loom.com/share/XXXXXXX"` |
| Vimeo | `"https://vimeo.com/XXXXXXX"` |

Optional thumbnail: `poster:"video/your-poster.jpg"`

A card with an empty `url` shows "Demo coming soon" instead of a Watch demo button. No other changes needed.

## Deploying

**Netlify** — drag the repository folder onto [app.netlify.com](https://app.netlify.com), or connect this repo for automatic deploys on every push.

**GitHub Pages** — Settings → Pages → Deploy from branch → `main` / root.

---

© Cherrylyn M. Alcaraz · Est. 2012
