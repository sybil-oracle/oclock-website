# O'Clock — Band Website

## What
Website mockup for O'Clock, a classic rock cover band based in the Wiener Neustadt area, Lower Austria. Bilingual (DE/EN), single-page, self-contained HTML.

## Status
**Mockup v2 — complete & shared for feedback** (2025-02-14)

## Decisions
- **Bilingual**: German default (Austria), English toggle via button top-right
- **Self-contained**: Single HTML file, no external dependencies except Google Fonts
- **Design**: Dark/warm palette (#2c2418 base, #8b2500 accent), Playfair Display + Source Sans 3
- **Sections**: Hero → About → Music → Shows → Gallery → Contact
- **Placeholder content**: All images are dashed-border placeholders, band members listed as "Member 1-4", show dates are fictional
- **Future hosting**: GitHub Pages (Juan needs to set up repo or give me access)

## Architecture
- Single HTML file with embedded CSS + JS
- Language toggle via `body.lang-de` class + `data-lang` attributes
- Fully responsive (mobile-friendly)
- Contact form is visual only (no backend)

## Bug Fixes Applied
- **v2**: `<a>` tags with `data-lang` weren't hiding properly — `.cta-btn` `display: inline-block` overrode lang rules. Fixed with `!important` and adding `a` to element-specific selectors.
- **v2**: German contact form lost flex layout — `display: block !important` from lang rules overrode `.contact-form` flex. Added specific `.contact-form[data-lang="de"]` rule.

## Assets (Google Drive)
- **Folder**: `Band Website Mockups` (ID: `14tmgw455EsTRTQbPnDjIdQfWTsVRPZlx`)
- Files:
  - `Band Website Mockup.html` — v1 (original)
  - `O'Clock Website Mockup.html` — v2 (intermediate)
  - `O'Clock Website Mockup v2 - FINAL.html` — v2 final (DE default, all fixes)

## Next Steps
- [ ] Collect feedback from bandmates
- [ ] Replace placeholder images with real band photos
- [ ] Fill in real member names, song titles, show dates
- [ ] Set up GitHub repo + GitHub Pages for permanent hosting
- [ ] Add real streaming links (Spotify, YouTube, SoundCloud)
- [ ] Hook up contact form to a backend (Formspree, Netlify Forms, or similar)
- [ ] Custom domain (e.g., oclock-rock.at)
