---
title: "GE szárítógép E-kódok: termisztorok, hőbiztosítékok és a fordulatszámjeladó"
description: "GE szárítógép E-kódok: E1, E3–E6, E4, E8, E11 — ajtókapcsoló, termisztorok, hőbiztosíték és motor, évjárat-csapdákkal és árakkal."
---

A GE azon kevés nagy háztartásigép-gyártó közé tartozik, amelyik nem tart fenn hivatalos hibakód-listát a szárítógépeihez. Az E-kódok léteznek, a vezérlőelektronika tárolja is őket — csak senki nem magyarázza el a tulajdonosnak, mit jelentenek. A rendszer mégis átlátható: a kódok négy terület köré tömörülnek, nevezetesen az ajtós áramkör, a két hőmérséklet-érzékelő, a fűtés biztonsági kioldói, valamint a meghajtómotor a fordulatszámjeladójával. A [GE szárítógép rovatunk](https://hu.codefixcoffee.com/ge/dryer/) kódonként részletesen tárgyalja mindet; ez a bejegyzés azt mutatja meg, hogyan áll össze a család egésszé, és mely évjáratoknál rejlenek a csapdák. Tájékozódni a [GE Appliances hivatalos honlapján](https://www.geappliances.com) is érdemes, például a használati utasításoknál.

## Olvassa ki először a tárolt kódot

2016 utáni GTD és GFD gépeken a legutóbb tárolt hibát maga is lekérdezheti. Kapcsolja ki a szárítógépet, nyomja le egyszerre a **Signal** és a **Temp** gombot, tartsa öt másodpercig a szervizmódhoz, és a kijelzőn megjelenik a friss hiba. SmartHQ-képes modelleknél az alkalmazás is listázza a tárolt kódokat. Ha csak a vezérlőelektronikát szeretné nullázni, húzza ki a gép dugóját öt percre.

## E1: az ajtókapcsoló

Az [E1](https://hu.codefixcoffee.com/ge/dryer/e1/) azt jelenti, hogy a vezérlőelektronika zártnak nem látja az ajtót. Ez jellemzően mechanikus, nem elektronikai hiba: kopott ajtózár, behajlított zárónyelv vagy egy már nem kattanó mikrokapcsoló.

- Nyomja határozottan be az ajtót, és indítsa újra — a félig beakasztott ajtó a leggyakoribb ok.
- Nézze meg az ajtó zárónyelvét: a behajlott vagy letört fület cserélni kell.
- Áramtalanítás után szerelje le az előlapot, és ellenőrizze az ajtókapcsoló csatlakozóját; amelyik kapcsoló megnyomásra már nem kattan, cserére szorul, €10–€25-ös alkatrészáron.

## E3–E6: a termisztorok

Két NTC hőérzékelő (termisztor) őrzi a légáram hőmérsékletét: a bemeneti a fűtőelem házán, a kimeneti a ventilátorházon ül. Az [E3–E6 család](https://hu.codefixcoffee.com/ge/dryer/e3-to-e6/) akkor lép fel, ha a vezérlőelektronika egyiküket szakadtnak vagy zárlatosnak látja. A gyakorlatban a laza, korrodált kábelcsatlakozás ugyanannyi esetet okoz, mint maga az elromlott érzékelő — és egy teljesen eltömődött szellőzőcső is képes egy egészséges gépet túlmelegíteni idáig.

1. Húzza ki a gépet 30 másodpercre, majd indítsa újra.
1. Tisztítsa meg a szűrőt, és győződjön meg róla, hogy a szellőzőcső nem szűkült-e el.
1. Nyissa fel a gépházat, és nézze után a termisztorok csatlakozóinak és kábelözésének laza vagy korrodált érintkezőit.
1. Mérje meg a termisztort multiméterrel: szobahőmérsékleten kb. 10 kΩ az egészséges érték; szakadt érzékelőt cseréljen.

A cserealkatrész €10–€25. Néhány típuson az E6 nem termisztor-, hanem légáramlás-hibakód, ezért rendelés előtt ellenőrizze a saját modellje kódlistáját.

## E4: a hőbiztosíték

Az [E4](https://hu.codefixcoffee.com/ge/dryer/e4/) a „nem fűt” jelzés: a dob forog, a ruha mégis vizes marad, mert egy biztonsági hőbiztosíték kiégett. A biztosíték sosem ok nélkül hal meg — a szűrőn vagy a szellőzőcsövön át nem távozó levegő engedte a fűtőelemet túlmelegedni. Előbb a légáramlást hozza rendbe, különben az új biztosíték is kiég, és soha ne hidalja át a hőbiztosítékot: ez az alkatrész az, amely egy valódi túlmelegedést megakadályoz abban, hogy tűzzé fajuljon.

1. Tisztítsa meg a szűrőt és a szabadba vezető teljes szellőzőszakaszt.
1. Mérje meg a hőbiztosítékot és a fűtőelemházán ülő hőhatároló termosztátot; amelyik szakadt, azt cserélje ki.
1. Futtasson egy rövid programot rövid időre leválasztott szellőzővel, hogy lássa, visszatér-e a meleg, majd csatlakoztassa vissza.

A hőbiztosíték €5–€15, a hőhatároló termosztát €10–€25.

## E8 és E11: a fordulatszámjeladó és a motor

Az [E8](https://hu.codefixcoffee.com/ge/dryer/e8/) a korszerű GE szárítógépeken a fordulatszámjeladó (tachometer) kódja: a vezérlőelektronika bekapcsolta a motort, de sebesség-visszajelzést sosem kapott. Az ok lehet a jeladó laza kábelezése, egy beragadt dob — lecsúszott szíj vagy a dob mögé került tárgy —, de a jeladó vagy maga a motor elromlása is. Mivel a tach a motoregység részét képezi, a bizonyított jeladóhiba egységes motorcserét jelent, €80–€150-ért; maga a szíj €15–€25.

Az E11 a szomszédos panasz: a motor nem azt teszi, amit a vezérlőelektronika kér — kopott szíj, megakadt dobgörgő vagy a motor indítókapcsolója, illetve maga a motor a hibás. Fordítsa meg kézzel a dobot: a nehézkes járás görgőkre vagy csapágyakra gyanakszik, nem a motorra. A szíj levétele után zümmögő, de el nem induló motor cserére szorul; a görgőszett €20–€40.

## Évjáratok szerinti csapdák

Három dologba szoktak belecsúszni a tulajdonosok. Először is: ugyanaz a szám nem minden gépen ugyanaz a hiba — egyes régebbi és kombi modelleken az E8 dobvilágítás- vagy leeresztési hibát jelent, nem fordulatszámjeladót, ezért alkatrészvásárlás előtt azonosítsa a saját szárítógépét. Másodszor: az E6 az egyik típuson légáramlási, a másikon termisztor-kód. Harmadszor: a fenti Signal+Temp szervizmód a 2016 utáni GTD/GFD gépekre vonatkozik — a korábbi modelleknél csak arra támaszkodhat, amit a kijelző a hiba pillanatában mutatott. A családhoz tartozik még az E7, amely azt jelzi, hogy a gép nem látja a táp mindkét fázisát, valamint az E14, a kezelőpanel beragadt gombja; egyik sem fűtési hiba.

## Mibe kerül a javítás?

Az érzékelő- és kapcsolószintű javítások olcsók: ajtókapcsoló €10–€25, termisztor €10–€25, hőbiztosíték €5–€15, szíj €15–€25, dobgörgő €20–€40. A drága tétel a meghajtómotor, €80–€150 — egy idősebb gépnél ez már mérlegelés kérdése, nem magától értetődő döntés. Szerelő kiszállása diagnózissal és alkatrésszel együtt kb. €120–€250; a motor körüli munkáknál megéri, ha nem szívesen nyitogatná a gépházat.

### Magyarországi használat: hálózat és szellőzés

Hazánkba a GE szárítógépek jellemzően amerikai importként érkeznek, és a típustöbbség 120/240 V, 60 Hz hálózatra készült — az itthoni 230 V, 50 Hz rendszertől eltérő paraméterekkel, így a bekötésüket bízza szakképzett villanyszerelőre. Panelházakban sokszor nincs mód szabadba menő szellőzésre, ott viszont épp a hosszú, áthajlított szellőzőcső válik az E3–E6 és E4 kódok leggyakoribb kiváltójává. Ahol csak lehet, alakítson ki rövid, egyenes kivezetést, és a szűrőt minden program után tisztítsa meg.
