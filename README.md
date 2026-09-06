# That's What She Said · The Office tribute

A compact editorial-style landing page celebrating The Office Telegram sticker pack
by artist Egor Zhgun. The original Russian and English page copy and artist attribution
are preserved in the product source.

**Status:** static frontend source. This is a tribute page; authorship of the sticker
artwork remains with its credited creator. Hosted availability has not been verified.

## Implementation highlights

- A self-contained HTML document with inline CSS and an inline SVG background illustration.
- Fluid typography and separate phone, tablet, and landscape layout adjustments.
- CSS entry animation and touch-specific hover behavior.
- A local hero image, descriptive alternative text, and links to the sticker pack and artist.
- Browser-native rendering with no JavaScript runtime or package dependencies.

## Source map

| File | Responsibility |
| --- | --- |
| [index.html](index.html) | Page content, responsive styling, inline SVG, and external links |
| [michael.png](michael.png) | Hero artwork credited to Egor Zhgun in the page |
| [.gitignore](.gitignore) | Local secret and session-file safeguards |

## Local preview

Requirements: Python 3 and a browser. From the repository root:

```sh
python -m http.server 8000 --bind 127.0.0.1
```

Open `http://127.0.0.1:8000`. The page can also be opened directly as `index.html`.
There is no dependency installation or build command.

## Maintenance guide

1. Edit content and styling in `index.html`; the document contains the complete layout.
2. Preserve the visible artist credit and the image alternative text when replacing artwork.
3. Check the heading, hero image, and two primary links at desktop and narrow phone widths.
4. Keep `michael.png` alongside the HTML when copying the site to a static host.

## Project references

- [The Office sticker pack](https://t.me/addstickers/ThatIsWhatSheSaid)
- [Egor Zhgun's channel](https://t.me/zhgun)

These are source references, not a claim of affiliation or ownership by the repository maintainer.

## Verification and boundaries

The existing [GitHub Pages demo](https://arar228.github.io/zhgun-office/) returned
HTTP 200 on 2026-09-07 and serves the root of `main`.

The documentation pass checks local file references and the static HTML entrypoint.
The repository contains no automated test suite or deployment workflow. Browser visual QA,
accessibility auditing, and external-link availability remain separate checks.

## Attribution and reuse

The existing page credits the sticker artwork to **Egor Zhgun**. The Office, its characters,
and associated names remain subject to their owners' rights. The repository has no license file;
public source availability does not grant a separate license to redistribute third-party artwork.
