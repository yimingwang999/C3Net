# C³Net — Qualitative Results

A static GitHub Pages project page with seven selected human–object interaction comparison videos.

## Contents

- Baseline: official N00 outputs.
- Ours: T02-50k outputs, not F01.
- Seven sampling modes, with front and two side-front views.
- No GT row. Each clip contains 10 saved frames displayed for 10 seconds.
- Original geometry and contact labels are unchanged.

## Selected Videos

| Mode | Selection |
| --- | --- |
| p(H \| O,I) | Retained previous selection |
| p(O \| H,I) | 010-02 |
| p(I \| H,O) | Retained previous selection |
| p(H,O \| I) | 110-04 |
| p(H,I \| O) | 101-02 |
| p(O,I \| H) | 011-03 |
| p(H,O,I) | 111-12 |

## Preview

Open `index.html` in a browser. No build step, external libraries, API keys or remote fonts are required.

## Publish on GitHub Pages

1. Review `DATA_NOTICE.md` and confirm permission to distribute the rendered assets.
2. Upload the contents of this folder to the root of the intended GitHub repository, preserving `assets/` and `videos/`.
3. In the repository, open **Settings → Pages**.
4. Choose **Deploy from a branch**, select the intended branch and **/(root)**, then save.
5. Open the site URL reported by GitHub Pages after deployment completes.

`.nojekyll` is included. All asset links are relative, including for project sites hosted under a repository subpath. No GitHub repository has been created or published by this package.

## Structure

```text
index.html
assets/style.css
assets/main.js
videos/               # Exactly seven MP4s and seven posters
manifest.json         # Source case identifiers and SHA-256 checksums
DATA_NOTICE.md
README.md
.nojekyll
```

## Interpretation

Presentation duration is not verified motion-capture duration. Source timestamps do not establish continuity; no interpolation is applied. Camera azimuths may differ between methods when humans are generated. Selected examples do not certify absence of penetration, temporal coherence, or superiority on every frame. See the page protocol and manifest for details.

## Display labels
The public presentation labels are Baseline and C³Net; their underlying results remain N00 and T02-50k respectively. Source-case banners are omitted from the videos, while provenance and checksums remain in manifest.json. Visualization limitations remain documented here.
