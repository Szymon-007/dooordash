# dooordash

Kamera przy drzwiach, która sama decyduje, kogo wpuścić. Działa na Jetson Orin Nano z kamerą IMX462, napisana w Pythonie.

Żeby wejść, trzeba przejść dwa kroki: kamera musi rozpoznać twarz domownika, a potem domownik pokazuje dłonią swój czteroznakowy kod. 

##

- **Twarz** – system zna domowników i odróżnia ich od obcych.
- **Kod z gestów** – każdy domownik ma własny kod, który pokazuje palcami do kamery.
- **Kod awaryjny** – drugi kod na wypadek, gdy ktoś zmusza domownika do otwarcia. Drzwi otwierają się normalnie, a właściciel dostaje alarm.
- **Dziennik** – zapis każdej próby wejścia: kto, kiedy i z jakim skutkiem.
- **Powiadomienia** – po każdej próbie na telefon właściciela idzie krótka wiadomość.
- **Panel** – strona w sieci domowej do zarządzania domownikami i kodami oraz przeglądania dziennika.

