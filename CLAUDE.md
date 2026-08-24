# Skrypt rozmowy windykacyjnej — Hadyński Inkaso

Interaktywny skrypt rozmowy dla windykatorów. Jedna strona HTML (`index.html`),
bez frameworków i bez builda — style, logika i wszystkie treści w jednym pliku.

## Produkcja i deploy

- **Adres: https://hadynski.github.io/dw-skrypt/**
- Hosting: GitHub Pages z brancha `main`, repo `Hadynski/dw-skrypt`
- **Deploy = `git push` na `main`.** Po ~1 minucie zmiana jest na produkcji.
- To repo NIE ma nic wspólnego ze stroną hadynski.pl ani ze skryptem M&B — nie mieszać.
- **Przed pushem zawsze `git fetch` + sprawdzić `origin/main`** — nad tym skryptem pracuje też
  Mikołaj z innych sesji i zdarzało się, że zdalnie była nowsza wersja (uwagi zespołu).
  W razie rozjazdu: rebase i zachować obie strony zmian, nigdy nie nadpisywać cudzych treści.

## Dostęp

- Wejście za hasłem zespołowym (ekran logowania, hasło zapamiętywane w przeglądarce).
- **Link bez wpisywania hasła:** hasło po `#` w adresie odblokowuje automatycznie
  (`https://hadynski.github.io/dw-skrypt/#<hasło>`) — to główny sposób dystrybucji dla zespołu.
- Na iPhonie warto „Dodaj do ekranu głównego" — Safari po ~7 dniach czyści pamięć strony
  i hasło wracało; aplikacja z ekranu głównego tego nie gubi.
- To bariera przed przypadkowymi osobami, nie kryptografia — repo jest publiczne.

## Zasady pracy nad treścią (ważne)

- **Wchodzi wyłącznie to, co Mikołaj zatwierdził na czacie.** Teksty rozmowy, sankcje i gałęzie
  powrotów przenosić 1:1 z jego notatek — bez „poprawiania" sensu, bez dopisywania obietnic.
- Propozycje treści najpierw w rozmowie do akceptu, dopiero potem wdrożenie.
- Ton: mówiony, konkretny, bez korporacyjnej waty.

## Konwencja wersji

- Commity numerowane wersjami: `v10.1`, `v10.2`, `v11: <krótko co i dlaczego>`.
- Przy zmianach treści podbijać wersję, żeby było wiadomo, kto co ma.

## Testowanie przed pushem

Sprawdzić składnię JS i przeklikać przepływ lokalnie (`python3 -m http.server`) —
wszystko jest w jednym pliku, więc jeden błąd w `<script>` kładzie całą stronę.
