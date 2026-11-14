# dooordash

Kamera przy drzwiach, która sama decyduje, kogo wpuścić. Działa na Jetson Orin Nano z kamerą IMX462, napisana w Pythonie.

Żeby wejść, trzeba przejść dwa kroki: kamera musi rozpoznać twarz domownika, a potem domownik pokazuje dłonią swój czteroznakowy kod. 

Cały projekt został wykonany bez robienia ctrl c ctrl v, wszystko za wyjatkiem readme bylo pisane przez człowieka, z ewentualna pomocą AI
##

- **Twarz** – system zna domowników i odróżnia ich od obcych.
- **Kod z gestów** – każdy domownik ma własny kod, który pokazuje palcami do kamery.
- **Kod awaryjny** – drugi kod na wypadek, gdy ktoś zmusza domownika do otwarcia. Drzwi otwierają się normalnie, a właściciel dostaje alarm.
- **Dziennik** – zapis każdej próby wejścia: kto, kiedy i z jakim skutkiem.
- **Powiadomienia** – po każdej próbie na telefon właściciela idzie krótka wiadomość.
- **Panel** – strona w sieci domowej do zarządzania domownikami i kodami oraz przeglądania dziennika.

## Rejestr użycia LLM

| Plik | Narzędzie | Do czego użyto i jak zweryfikowano |
| --- | --- | --- |
| `.github/workflows/ci.yml` | Claude | Treść zaproponowana przez Claude'a i omówiona linijka po linijce; przepisana ręcznie, wersje akcji sprawdzone w Releases, działanie potwierdzone zielonym przebiegiem pipeline'u. |
| `.github/workflows/release.yml` | Claude | Treść zaproponowana przez Claude'a i omówiona linijka po linijce; przepisana ręcznie, działanie sprawdzone próbnym tagiem `v0.0.1`. |
