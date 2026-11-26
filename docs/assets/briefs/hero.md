# Brief: README hero and social preview

Date: 2026-11-26. Output: `docs/assets/hero-art.png` (AI illustration, no text), composed with real type into `docs/assets/hero.jpg` (README banner) and `docs/assets/social-preview.jpg` (1280x640, upload in GitHub Settings, Social preview). The exact prompt, model and time are in `docs/assets/hero-art.png.json`. References are inspiration only; none was used as an image input or copied.

## What a newcomer must see
Normal behaviour forms a dense, regular baseline; the models flag the few events that fall outside it, and a risk score ranks users.

## References
| Reference | What works | Taken / avoided |
|---|---|---|
| [OpenUBA](https://github.com/GACWR/OpenUBA) (opened) | Mural hero above the title, layered architecture SVG with a layer table | Hero first, then a diagram. Avoided its dense badge row |
| [notabombe/OpenUBA](https://github.com/notabombe/OpenUBA) (opened) | One clear scope sentence: observe events and anomalies, not replace a SIEM | Put scope in the README text, not the art |
| [Raoof128/ITDE](https://github.com/Raoof128/ITDE) (search snippet only, page returned 404) | Ingest, baseline, detect, score, alert as stages | Matches the Mermaid flow added to the README |

Research note: the references show UBA READMEs lean on a diagram plus a layer or stage table; I found no illustrated hero that explains the method, so the art shows the method itself (baseline vs outliers).

## Design (revised 2026-11-26)

- **Style:** Painterly dusk (gouache and oil texture).
- **Why this picture:** Behaviour analytics learns what the flock normally does and flags the one that leaves it. A murmuration with one red bird says that at a glance.
- **Subject:** a flowing murmuration of hundreds of dark starling silhouettes across a violet, magenta and burnt-orange sunset, with one vermilion bird on its own path and a thin trail. Palette: violet, magenta, orange, one red accent.
- **Layout:** the left third stays quiet for the title; colours and font of the title are set per image in `compose_banner.py`.
- **Must not contain:** text, letters, numbers, logos, watermarks, borders, real people, robots.
- **QA:** schema check by a vision model against this brief, plus a manual look.

## Revision note

The first version of this banner used the same dark navy, teal and grid look as the owner's other repos. It was consistent but samey, so it was replaced with a distinct art direction per repo, each built on a metaphor for what the repo does.
