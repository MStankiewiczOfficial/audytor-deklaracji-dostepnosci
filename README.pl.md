# Audytor Deklaracji Dostępności

Interaktywne narzędzie do ręcznego audytu deklaracji dostępności (zgodność z Warunkami Technicznymi publikacji deklaracji). Pozwala:

- wkleić treść deklaracji (HTML lub tekst),
- wstępnie wykryć istotne sekcje i elementy,
- przejść listę kontrolną i ocenić zgodność („Spełnione / Niespełnione / Nie dotyczy”),
- obliczyć procent zgodności i ocenę opisową,
- zapisać szkic lokalnie (localStorage),
- eksportować wynik do JSON lub HTML (raport).

## Jak uruchomić lokalnie

Wystarczy otworzyć plik `index.html` (lub `audyt-deklaracji.html`) w przeglądarce. Nie są potrzebne żadne zależności ani serwer.

## Publikacja (GitHub Pages)

1. Upewnij się, że plik `index.html` jest w katalogu głównym repozytorium.
2. Włącz GitHub Pages w ustawieniach repozytorium (Settings → Pages → Source: Deploy from a branch, Branch: `main` / root).

## Prywatność

- Aplikacja działa w 100% po stronie przeglądarki. Wklejone dane nie opuszczają Twojego urządzenia.
- Szkice są przechowywane lokalnie w `localStorage` pod kluczem `audyt-deklaracji-szkic`.

## Licencja

CC BY-NC-SA 4.0. Zobacz plik `LICENSE`.
