# O'Clock — Band Website

## What
Website for O'Clock, a classic rock cover band based in the Wiener Neustadt area, Lower Austria. Bilingual (DE/EN), single-page, self-contained HTML.

## Status
**v3 — Live on GitHub Pages** (2026-02-15)

## Live URL
https://sybil-oracle.github.io/oclock-website/

## GitHub Repo
https://github.com/sybil-oracle/oclock-website (public)

## Changes in v3
- Background color changed from cream (#f5f0e8) to warm orange (#EAA741) per band feedback
- Added Beatles mention in About text
- Fixed nav bar contact button hidden behind language toggle (added nav padding)
- Added section toggle system (JS config at bottom of index.html)
- Adjusted card/placeholder colors for contrast against new background
- Removed mockup note badges
- Shows section hidden by default (toggle in JS)

## Section Toggle System
At the bottom of `index.html`, there's a `SECTIONS` config object:
```js
const SECTIONS = {
  about:   true,
  music:   true,
  shows:   false,   // hidden until confirmed events
  gallery: true,
  contact: true,
};
```
Set any section to `false` to hide it (and its nav link).

## Media Workflow
1. **Google Drive upload folder**: [O'Clock Website Media](https://drive.google.com/drive/folders/1OULSrjzGF8ZUcpnN_Jsi7i1YT2i6_XxO)
   - Subfolders: `hero/`, `about/`, `gallery/`, `music/`, `members/`
   - Band members can upload directly; see README in folder for naming convention
2. **Sync to repo**: Tell Sybil "new photos uploaded" → pulls from Drive, commits to repo
3. **GitHub Pages auto-deploys** on push

## Drive Folder IDs
- Media root: `1OULSrjzGF8ZUcpnN_Jsi7i1YT2i6_XxO`
- hero: `1c7rCa1Cgw4SSd-wp0J2TMjdeZgqAreBz`
- about: `18_0aTAkYPVKnn-By41klH7pEABCJVvuR`
- gallery: `1jcVIKrvZM0z6h9nDk0699unhXbmV8PsV`
- music: `1MrelyGvrIYT1r1nOh2k8yBW-qjfiOTz8`
- members: `1FKBK-bu_ugNzGeu9YpbPe96GhOdRnx8I`

## Next Steps
- [ ] Enable GitHub Pages (Juan needs to do this manually — Settings > Pages > main branch)
- [ ] Add custom domain (oclock-rock.at or similar)
- [ ] Replace placeholder images with real photos
- [ ] Fill in real member names, song titles, show dates
- [ ] Hook up contact form backend (Formspree or similar)
- [ ] Add real streaming links
