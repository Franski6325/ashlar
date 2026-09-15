# Ashlar Lab

Personal design portfolio of **fictional** single-file landing pages — GSAP, ScrollTrigger, Lenis, original copy and CSS/SVG graphics.

The repository root `index.html` is the catalog. Each plane lives in `sites/<nn>-<slug>/index.html`. The studio study is `sites/00-ashlar/`.

## Layout

```
index.html              ← catalog (lab home)
sites/00-ashlar/        ← studio landing
sites/01-deckle/ … 31-voltabit/
sites/index.html        ← redirect to the catalog
```

Old catalog names that never matched folders (Vellum, Relay, Volta, Arc, Facet) now point at the live directories: Deckle, Murmur, Citrine, Stillpoint, Tessera.

## Disclaimer

Ashlar Lab is a personal design portfolio of **fictional** brand systems and landing-page studies. Every product name, company, metric, and story here is invented for demonstration. Nothing is affiliated with, endorsed by, or related to any real company that may share a similar name — including, without limitation, Ashlar-Vellum CAD software or any other trademark holder. These pages are not offers of goods, services, banking, medical advice, energy services, or security products.

Forms and checkout UIs are demos only; they do not process payments or send email.

## Third-party libraries

| Library | Use | Notes |
|---------|-----|--------|
| [Google Fonts](https://fonts.google.com/) | Typography | OFL / Apache licenses via CDN |
| [GSAP](https://gsap.com/) 3.12.5 + ScrollTrigger | Motion | Free Standard License (core + ScrollTrigger); no Club plugins |
| [Lenis](https://github.com/darkroomengineering/lenis) | Smooth scroll | MIT via CDN |

## Local preview

Serve the **repository root** (not the `sites` folder):

```bash
npx --yes serve .
```

Then open `/` for the catalog and `/sites/00-ashlar/` for the studio.

## Cloudflare

Workers Builds runs `npx wrangler versions upload`. This repo is a static HTML catalog (no Worker script). `wrangler.jsonc` points assets at the repository root; `.assetsignore` keeps `.git`, `.github`, and similar files off the public site.

## License

Portfolio code and original writing in this repository are released under the MIT License (see `LICENSE`). Third-party fonts and libraries remain under their own licenses.
