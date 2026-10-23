# Presto Presto · www.presto-presto.it

"Coming soon" page for **Presto Presto**, coffee and pasta to go ("Pasta fresca espressa · Caffè italiano autentico").
Client: Davide Schiano Lo Moriello and partner. Instagram: [@prestopresto.it](https://www.instagram.com/prestopresto.it/).
Built by **IT-Konsulent Tavassoli** (Babak Tavassoli) · it.konsulent@yahoo.com.

| | |
|---|---|
| Live page | https://www.presto-presto.it (bare domain and http redirect to it) |
| Hosting | **Aruba hosting** (Hosting Gestito Smart per WordPress) since 23 Oct 2026: `index.html` and `logo.svg` in the web root, `.htaccess` starts with `DirectoryIndex index.html index.php` so the static page is served instead of the untouched WordPress install. After every upload: Aruba panel → Velocità → Caching → cancella cache. GitHub Pages from this repository stays as a backup. |
| Important | GitHub Pages on the **Free** plan only works while this repository is **public**. Making it private takes the page offline unless the account is on GitHub Pro or the page moves to other hosting. |
| Domain / DNS | presto-presto.it at Aruba ("Dominio con email", account 17170731@aruba.it). **Expires 5 Nov 2026**: Davide must renew. |
| DNS set 16 Oct 2026 | `A @` → 185.199.108.153, .109.153, .110.153, .111.153 · `CNAME www` → pbtmail.github.io. Old values: `A @` 62.149.128.40, `CNAME www` → presto-presto.it. All mail records untouched. |

## Files
| Path | What it is |
|---|---|
| `index.html` | The page: official logo, "Stiamo arrivando… presto presto", three features, Instagram link. Colours and type follow the logo guideline. |
| `CNAME` | `www.presto-presto.it` for GitHub Pages. Do not delete. |
| `logo.svg` | **Official** vertical logo for dark backgrounds, cut as vector from the cover of `brand/LogoGuideline_PrestoPresto.pdf`. |
| `brand/` | Logo guideline from Davide's designer (Adobe Illustrator PDF, 5 pages: configurations, colours, use on light/dark, fonts) and the extracted SVG. |
| `src/post.jpg` | The 1440 px Instagram post (source of colours, copy and photo). |
| `src/index-v2-orange-redrawn-logo.html` | Earlier version: orange background with my redrawn logo (before the guideline arrived). |
| `src/index-v3-instagram-post.html` | Fuller version built from the whole Instagram post; parked by Babak ("keep it simple for now"). Needs `food.webp`: crop `src/post.jpg` x 700–1440, convert with `cwebp -q 72`, 421×820. |
| `docs/claude/` | Memory note and text-only log of the Claude conversation. |

## Update the page
Edit `index.html` (GitHub web editor is fine), commit to `main`; GitHub Pages republishes within a minute or two.

## Going back to GitHub Pages
In the Aruba DNS panel set `A @` to 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153 and `CNAME www` → `pbtmail.github.io`, then re-check the custom domain in the repository's Pages settings.

## Brand rules (from the guideline)
- Colours: orange #cc6533 (renders as #ED592D in the PDF), dark #333334 (cover background #231F20), light #ebe8eb, green #336637, red #c73635.
- Logo: orange on white or dark backgrounds; white or black versions for one-colour use. Not on orange.
- Font: Puffin Display Soft Bold (Adobe Fonts). Titles orange, slanted 10°; subtitles black or white, letter-spacing 45. The page uses Baloo 2 as a free stand-in.
