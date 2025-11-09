# Accessibility Declaration Auditor

An interactive, client‑side tool to audit accessibility declarations (compliance with the Polish "Warunki Techniczne" – technical requirements for publishing the accessibility statement).

Key features:
- paste the declaration (HTML or plain text)
- quick keyword pre‑detection of required sections
- go through a checklist and mark: Met / Not met / Not applicable
- auto score (compliance %) and descriptive label
- local draft save (localStorage)
- export results to JSON or printable HTML report

## Run locally
Just open `index.html` (or `audyt-deklaracji.html`) in your browser. No server or dependencies required.

## Publish (GitHub Pages)
1. Ensure `index.html` sits in the repository root.
2. Enable GitHub Pages (Settings → Pages → Source: GitHub Actions). A ready workflow is in `.github/workflows/pages.yml`.

## Privacy
- 100% client‑side. Pasted data never leaves your device.
- Drafts are stored locally in `localStorage` under the key `audyt-deklaracji-szkic`.

## Reference: official requirements (Warunki Techniczne)
- Ministry of Digital Affairs: "Warunki techniczne publikacji oraz struktura dokumentu elektronicznego deklaracji dostępności" (in Polish):
  https://mc.bip.gov.pl/objasnienia-prawne/warunki-techniczne-publikacji-oraz-struktura-dokumentu-elektronicznego-deklaracji-dostepnosci.html

## License
This project is licensed under CC BY‑NC‑SA 4.0. See `LICENSE`.

## Third‑party licenses
- Bootstrap 5 (CDN) — MIT License: https://github.com/twbs/bootstrap/blob/main/LICENSE
  - If you redistribute Bootstrap files yourself (instead of using a CDN), keep the MIT license notice.
