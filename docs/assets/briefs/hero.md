# Brief: README hero and social preview

Date: 2026-11-26. Output: `docs/assets/hero-art.png` (AI illustration, no text), composed with real type into `docs/assets/hero.png` (README banner) and `docs/assets/social-preview.png` (1280x640, upload in GitHub Settings, Social preview). The exact prompt, model and time are in `docs/assets/hero-art.png.json`. References are inspiration only; none was used as an image input or copied.

## What a newcomer must see
Normal behaviour forms a dense, regular baseline; the models flag the few events that fall outside it, and a risk score ranks users.

## References
| Reference | What works | Taken / avoided |
|---|---|---|
| [OpenUBA](https://github.com/GACWR/OpenUBA) (opened) | Mural hero above the title, layered architecture SVG with a layer table | Hero first, then a diagram. Avoided its dense badge row |
| [notabombe/OpenUBA](https://github.com/notabombe/OpenUBA) (opened) | One clear scope sentence: observe events and anomalies, not replace a SIEM | Put scope in the README text, not the art |
| [Raoof128/ITDE](https://github.com/Raoof128/ITDE) (search snippet only, page returned 404) | Ingest, baseline, detect, score, alert as stages | Matches the Mermaid flow added to the README |

Research note: the references show UBA READMEs lean on a diagram plus a layer or stage table; I found no illustrated hero that explains the method, so the art shows the method itself (baseline vs outliers).

## Design
- **Subject:** a translucent teal sphere filled with regular flow lines and nodes (the behaviour baseline), with three amber points outside it joined by thin dotted lines (anomalies).
- **Palette and style (shared across the owner's repos):** deep navy ink (#0B1020), teal/green highlight, amber for the exception, soft glow, faint perspective grid, minimal and not photoreal. Subject in the right two-thirds, calm empty left third for the title.
- **Must not contain:** text, letters, numbers, logos, watermarks, borders, people, robots, brains.
- **QA:** schema check by vision model against this brief, plus a manual look. Result noted in the commit.
