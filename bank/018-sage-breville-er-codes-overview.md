---
title: "Sage/Breville ER hibakódok: a rejtett szerviztáblázat olvasása"
description: "A Sage és Breville ER kódjai nem publikus szerviztáblából jönnek. Az ER01–ER18 felépítése és az Oracle eltérő számozása."
---

Ha a Breville kávégép leáll, és a kijelzőn ER05 látható, a használati utasításból hiába keresi a magyarázatot. Ez nem elnézés a szerkesztők részéről: a Breville hibakódjai azokból a belső szerviztáblákból származnak, amelyeket a cég a javításokhoz használ, de a vásárlóknak nem ad ki. Ugyanez a hardver Nagy-Britanniában **Sage** márkanéven fut — a gépek azonosak, csak a felirat más —, ezért a Sage Barista Touch ER-kódjai pontosan azt jelentik, amit a Breville példányokon. A [Breville / Sage rovatunk](https://hu.codefixcoffee.com/breville/) az aktuális modellválasztékot foglalja össze; ez a bejegyzés a számozás rendjét világítja meg, hogy egy sosem látott kódból is kiolvashasson valami hasznosat.

## Miért nem publikálja őket a Breville

A felhasználói kézikönyv a tisztítást és a mészetlenítést tárgyalja, a hibakeresést nem. A teljes kódtáblázatok az egyes gépek szerviz módjában rejtőznek: jelszóval védett, szerviztechnikusoknak szánt képernyőkön, eltárolt hibaszámlálókkal és élő érzékelőadatokkal. Mivel a kódok javítóeszköznek készültek, nem fogyasztói funkciónak, a Breville soha nem adta ki őket nyilvános dokumentumban — a legtöbb tulajdonos egyetlen kódot lát életében, azt is, amelyik a leállást okozta. A kontraszt a Miele-nél éles: ők kinyomtatják az F-kódok jelentését a használati utasításba, éppen ezért tudnak a [Miele kódoldalaink](https://hu.codefixcoffee.com/miele/) a kézikönyvre hivatkozni.

## A Barista Touch táblázat: ER01-től ER18-ig

A Barista Touch (BES880) és a Barista Touch Impress (BES881) — utóbbi ugyanazt a vezérlőelektronika-családot és kódtáblát örökli — tizennyolc bejegyzéses táblázattal dolgozik. A felépítés átlátható, ha egyszer megvan a kulcsa: az érzékelők kódjai **négyes csoportokban** érkeznek, érzékelőnként egy-egy csoport, sorban induláskori nyitott kör, üzem közbeni nyitott kör, majd a két rövidzárlatos eset.

- **ER01–ER04** — a ThermoJet („ferro”) fűtő hőérzékelője a négy nyitott kör / rövidzárlat változatban; az [ER01](https://hu.codefixcoffee.com/breville/barista-touch-bes880/er01/) az induláskori nyitott kör bejegyzése.
- **ER05–ER08** — a tejkancs hőérzékelője, a cseppgyűjtő környékén ülő kis szonda, amely gőzöltetés közben a kancs hőmérsékletét méri. Az ER05, az induláskori nyitott kör, a Barista Touchon leggyakrabban jelentett kód, és mind a négy bejegyzés ugyanazt a javítást igényli.
- **ER09–ER12** — a sorba épített, a főzővizet mérő hőérzékelő, ugyanazzal a négyes mintával.
- **ER13 és ER14** — áramlásmérő-számlálási hibák induláskor és üzem közben: a szivattyú futott, a gép mégsem tudta megszámolni az átáramló vizet.
- **ER15** — kommunikációs hiba a belső elektronikus modulok között; sokszor kilazult szalagkábel vagy nedves csatlakozó, nem feltétlenül elhalt panel.
- **ER16 és ER17** — a daráló: a motor túlmelegedett és védelemből leállt, illetve a motor a feladatát időre nem tudta befejezni.
- **ER18** — E-fast védelem: elektromos vagy biztonsági hiba, például szivárgó áram; ez az a kód, amely a konnektor mögötti áramvédő kapcsolót (RCD-t) is kiütheti.

## Az Oracle család másképp számoz

Oracle-vásárlással ugyanez az elv hosszabb táblán folytatódik. Az Oracle (BES980) és az Oracle Touch (BES990) közös, 32 bejegyzéses listán osztozik, de a BES980 „Error 1”-től „Error 32”-ig számoz, a BES990 pedig ER-előtagot tesz a kódok elé. Az első tizenhat a kvartett-logikát négy érzékelőre alkalmazza — gőzkazán-kódok az 1-től 4-ig, kávékazán-kódok az 5-től 8-ig (az [Error 8](https://hu.codefixcoffee.com/breville/oracle-bes980/error-8/) a kávékazán-érzékelő üzem közbeni rövidzárlata), fűtött fejrész a 9-től 12-ig, gőzkar a 13-tól 16-ig. A maradék bejegyzések: nem melegedő kazánok (17–19), gőzkazán-szint- és töltéshibák (20 és 21), áramlásmérő-problémák (22 és 23), szintszondák és túlmelegedés (24–27), panelkommunikációs hiba (28), daráló (29 és 30), tömörítőmotor (31), valamint gőzkazán-szivárgás vagy sikertelen újratöltés (32).

Két kisebb tábla teszi teljessé a családot. Az Oracle Jet (BES985) saját, rövidebb E1–E19 tábláját használja, a Dual Boiler (BES920) pedig kétjegyű, 00-tól 12-ig számozott kódjait nem a normál kijelzőn, hanem egy rejtett önteszt menüben őrzi — egy Dual Boiler így olyan hibán is ülhet, amelyet a kijelzőn sosem látott.

## A rejtett hibanapló saját kezű olvasása

A táblák szervizadatok, így a gép előzményeit is ugyanazon a szervizképernyőn keresztül érheti el. Az útvonalak technikushangulatúak, de a javítók jól dokumentálták őket:

- **Barista Touch és Oracle Touch** — kapcsolja ki a falnál, tartsa nyomva az elülső Power gombot, miközben visszakapcsolja a fali kapcsolót, engedje el a logó felbukkanásakor, adja meg a 00000 szervizjelszót, majd nyissa meg az Error Countert a tárolt hibákhoz vagy a Live Debugot az élő hőmérsékletekhez és vízszintekhez.
- **Barista Touch Impress** — ugyanaz a gombkombináció, csak a szervizjelszó 02015.
- **Oracle BES980** — bedugott, kikapcsolt gépnél tartsja legalább egy másodpercig egyszerre az 1 CUP, 2 CUP és POWER gombokat; a hosszú sípolás után a SELECT gomb megnyitja az Error Storage-t, amelyben mind a 32 kód és a tárolt darabszámok végigléptethetők.

Ezeket a képernyőket kizárólag olvasásra kezelje: jegyezze fel, mi van tárolva, a beállításokhoz ne nyúljon, és a naplót csak a javítás után törölje — csak így tudja eldönteni, hogy egy kód visszatér-e.

## Mibe kerül a javítás

Közzétett tábla nélkül is kiszámítható a számtan. A hőérzékelő-szerelvények €25 és €95 közé esnek, attól függően, melyik szondáról van szó (a gőzkaros és a tejkancsos a drágábbak), az O-gyűrűs szettek €10–€20 közé; a tejszonda-javítókészlet €30–€50, a gyári szerelvény €80–€95. Garancián kívüli gyári ajánlatok belső hibákra jellemzően €300–€500 körül mozognak, így az érzékelőszintű javítás független műhelyben általában a jobb út. A Sage-feliratú gépek ugyanezen tábláinak lefedettségét a [webhely brit kiadása](https://hu.codefixcoffee.com/uk/) adja.

### Mire számítson, ha itthon Sage gépe van

A Sage gépek Magyarországon nem hivatalos disztribúcióban érhetők el: a legtöbb itthoni példány brit import. A feszültség szerencsére stimmel (230 V, 50 Hz), a brit G típusú villásdugasz viszont a magyar aljzatokba nem illik — használjon jó minőségű átalakítót, vagy csereasztal mellett cseréltessen dugaszt. A gépek angol nyelvű útmutatói a [Sage hivatalos támogatási oldalán](https://sageappliances.co.uk) érhetők el, szervizeléshez pedig itthon a független kávégépjavító műhelyek jelentenek reális útvonalat.
