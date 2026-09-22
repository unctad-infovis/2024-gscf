# 2024-gscf

## About

Hosts video and poster-image assets for UNCTAD's 2024 Global Supply Chain Forum — a press-release video, a general event video, and several numbered/alt cuts (each as `.mp4`/`.webm` pairs for cross-browser playback), plus their poster-frame `.jpg` images.

Asset-hosting repo only — there is no page here, no `src/`, and no build tooling. `public/` is synced directly to production.

## Rights of usage

Contact Teemo Tebest.

## Files and folders

* `public/assets/vid/` — event and press-release videos (`.mp4` + `.webm` per clip)
* `public/assets/img/` — poster-frame images for the videos

## Hosting

No build step — `npm run sync-prod` copies `public/*` directly to `https://storage.unctad.org/2024-gscf/` via `azcopy`; `npm run sync-gh-pages` mirrors `public/` to this repo's GitHub Pages branch.
