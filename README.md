# telefon
Telefonok beszedését és kiadását adminisztráló alkalmazás

A program célja
~~~~~~~~~~~~~~~
A telefonok ki- és beadásának adminisztrációját gyorsan és egyszerűen végezze.

Használata:
~~~~~~~~~~
- Megjelenik egy bejelentkezési ablak
  https(s)://[url]

- Átlagos felhasználó / Adminisztrátor

Funkciók:
========

Felhasználóknak be kell jelentkezniük.

Felhasználó (bejelentkezés után)
~~~~~~~~~~~
- Telefon beolvasása kamerával (mobilon, fájlból PC-n)
  Azonosítja a telefont és betölti az adatait

- Egy telefon beadása / kiadás
  https(s)://[url]?id=TelefonAzonosító
  A felületen megjelenik a telefon az esemény utáni pillanatnyi állapota.
  Két gomb jelenik meg Bevét / Kiadás
  Ha az eszköz nincsen bejelentkezve, akkor csak a pillanatnyi állapot, de nincsen be- és kivét.

- Egy telefon állapotának lekérdezése (események)
  https(s)://[url]?id=TelefonAzonosító&cmd=view
  A felületen megjelenik a telefon pillanatnyi állapota és a korábbi események időben fordított sorrendben

- Telefonok listázása

- Kilépés

Adminisztrátor
~~~~~~~~~~~~~~
- Új telefon felvétele az adatbázisba
  https(s)://[url]?cmd=new
  Megjelenik az adatbeviteli felület és a telefon adatait kitöltve lehet bevinni az adatbázisba az adatokat.

- Telefonok importálása Excel (csv) fájlból

- Egy telefon adatainak módosítása
  https(s)://[url]?id=TelefonAzonosító&cmd=mod
  A felületen megjelenik a telefon pillanatnyi állapota és a mezőkbe írt adatok módosíthatók.

- Telefon (logikai) törlése az adatbázisból
- QRCode létrehozása: Egy telefon adatából QR kódot generálunk automatikusan.
- Telefonok listázása: https(s)://[url]?cmd=Lista - Az adatbázisban lévő telefonok alapadatainak listája

Felhasználók kezelése
~~~~~~~~~~~~~~~~~~~~~
- Felhasználók listázása
- Egy felhasználó kiválasztása => adatainak módosítása
- Egy felhasználó jelszavának módosítása. A jelszavak elkódolva vannak az adatbázisban
- Felhasználók nagy tümegű importálása Excel (csv) fájlból
- Felhasználó törlése (logikai / fizikai)
