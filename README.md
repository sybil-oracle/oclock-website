# O'Clock — Band Website

## What
Website for O'Clock, a classic rock cover band based in the Wiener Neustadt area, Lower Austria. Bilingual (DE/EN), single-page, self-contained HTML.

## Status
**v4 — Live on GitHub Pages** (2026-02-18)

## Live URL
https://sybil-oracle.github.io/oclock-website/

## GitHub Repo
https://github.com/sybil-oracle/oclock-website (public)

## Band Members
- **Freddy** — Lead Guitar
- **Juan** — Bass
- **Karl** — Vocals / Rhythm Guitar
- **Christine** — Drums

## Changes in v4
- Replaced all placeholder images with real media from Google Drive
- Hero: band logo (cropped tight, larger display)
- About: real group photo
- Gallery: 6 live shots (Sollenau Rock + Traiskirchen) with hover zoom
- Music: 3 playable audio tracks (Jumping Jack Flash, Born to Be Wild, Ain't No Sunshine) with native HTML audio players
- Real member names added (both DE/EN)
- Streaming note changed to "Bald" / "Coming soon" (not yet on platforms)
- Section dividers darkened for visibility against orange background
- Social media links hidden (no accounts yet)
- Booking note restyled for better readability (dark brown, bold)
- Music section subtitle changed to "Live recordings"

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
- [ ] Add custom domain (oclock-rock.at or similar)
- [ ] Create social media accounts (IG, YT, FB) and unhide links
- [ ] Upload to streaming platforms and update "Bald" note
- [ ] Fill in real show dates and enable Shows section
- [ ] Get more member photos for a dedicated members section
- [ ] Hook up contact form backend (Formspree or similar)
- [ ] Add more gallery photos as gigs happen
