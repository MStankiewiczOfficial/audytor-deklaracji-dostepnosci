# Audytor Deklaracji Dostępności

Interaktywne narzędzie do ręcznego audytu deklaracji dostępności (zgodność z Warunkami Technicznymi publikacji deklaracji). Pozwala:

- wkleić treść deklaracji (HTML lub tekst),
- wstępnie wykryć istotne sekcje i elementy,
- przejść listę kontrolną i ocenić zgodność („Spełnione / Niespełnione / Nie dotyczy”),
- obliczyć procent zgodności i ocenę opisową,
- zapisać szkic lokalnie (localStorage),
- eksportować wynik do JSON lub HTML (raport).

Dodatkowe informacje:
- Tryb ciemny: aplikacja zawiera przełącznik jasny/ciemny i domyślnie podąża za preferencją systemową (prefers-color-scheme). Kolory zostały dostrojone pod kątem kontrastu, jednak zalecamy wizualną weryfikację dla Twoich treści.
- Dostępność: interfejs wykorzystuje semantyczne elementy HTML (fieldset/legend), atrybuty ARIA oraz regiony live, żeby poprawić obsługę klawiatury i czytników ekranu.
- Ikony: w UI wykorzystywane są Bootstrap Icons (serwowane z CDN). Jeśli zdecydujesz się je hostować samodzielnie, pamiętaj o dołączeniu informacji o licencji MIT.
- Klucze localStorage: szkice zapisywane są pod `audyt-deklaracji-szkic`, a preferencja motywu pod `audyt-theme-preference`.

## Jak uruchomić lokalnie

Wystarczy otworzyć plik `index.html` w przeglądarce. Nie są potrzebne żadne zależności ani serwer — to pojedynczy statyczny plik HTML.

## Publikacja (GitHub Pages)

1. Upewnij się, że plik `index.html` jest w katalogu głównym repozytorium.
2. Włącz GitHub Pages w ustawieniach repozytorium (Settings → Pages → Source: Deploy from a branch, Branch: `main` / root).

> [!TIP]
> Przed publikacją sprawdź linki CDN do Bootstrap i Bootstrap Icons, jeśli środowisko blokuje zewnętrzne zasoby.

## Prywatność

- Aplikacja działa w 100% po stronie przeglądarki. Wklejone dane nie opuszczają Twojego urządzenia.
- Szkice są przechowywane lokalnie w `localStorage` pod kluczem `audyt-deklaracji-szkic`.

## Odnośnik: oficjalne wymagania (Warunki Techniczne)
- Ministerstwo Cyfryzacji: "Warunki techniczne publikacji oraz struktura dokumentu elektronicznego deklaracji dostępności":
	https://mc.bip.gov.pl/objasnienia-prawne/warunki-techniczne-publikacji-oraz-struktura-dokumentu-elektronicznego-deklaracji-dostepnosci.html

## Licencja
Projekt jest licencjonowany na zasadach CC BY‑NC‑SA 4.0. Zobacz plik `LICENSE`.

## Licencje osób trzecich
- Bootstrap 5 (CDN) — licencja MIT: https://github.com/twbs/bootstrap/blob/main/LICENSE
	- Jeśli samodzielnie dystrybuujesz pliki Bootstrap (zamiast korzystać z CDN), dołącz informację o licencji MIT.
 - Bootstrap Icons (CDN) — licencja MIT: https://github.com/twbs/icons/blob/main/LICENSE
	- Jeśli hostujesz pliki ikon lokalnie, dołącz odpowiednią informację o licencji MIT.