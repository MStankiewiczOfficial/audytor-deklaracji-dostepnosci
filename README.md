# Accessibility Declaration Auditor

An interactive, client‑side tool to audit accessibility declarations (compliance with the Polish "Warunki Techniczne" – technical requirements for publishing the accessibility statement).

Key features:
- paste the declaration (HTML or plain text)
- quick keyword pre‑detection of required sections
- go through a checklist and mark: Met / Not met / Not applicable
- auto score (compliance %) and descriptive label
- local draft save (localStorage)
- export results to JSON or printable HTML report

Additional notes:
- Dark mode: the app includes a dark/light theme toggle and follows the system preference (prefers-color-scheme). Color tokens were tuned for good contrast but please verify visually for your content.
- Accessibility: the UI uses semantic HTML (fieldset/legend, ARIA attributes, live regions) and focus-visible styles to improve keyboard and screen-reader use.
- Icons: Bootstrap Icons are used for small UI badges and glyphs (served from CDN). If you self-host the icons, keep the MIT license notice.
- LocalStorage keys: drafts are saved under `audyt-deklaracji-szkic` and theme preference under `audyt-theme-preference`.

## Run locally
Just open `index.html` in your browser. No server or build step required — it's a single static HTML file.

## Publish (GitHub Pages)
1. Ensure `index.html` sits in the repository root.
2. Enable GitHub Pages (Settings → Pages → Source: Deploy from a branch, Branch: `main` / root).

> [!TIP]
> When publishing, double-check the CDN links for Bootstrap and Bootstrap Icons if your environment blocks external assets.

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
 - Bootstrap Icons (CDN) — MIT License: https://github.com/twbs/icons/blob/main/LICENSE
  - If you self-host the icon files, keep the MIT license notice.
