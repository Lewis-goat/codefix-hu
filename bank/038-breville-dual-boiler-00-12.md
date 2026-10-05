---
title: Breville Dual Boiler 00–12: a kétszámjegyű kódok
description: A Breville Dual Boiler BES920 kódjai (00–12) egy rejtett tesztmenüben olvashatók: mit jelent a kód, és a gőz- vagy a főzőoldal hibája-e.
---

A Breville kávégépeinek többsége a megszokott kijelzőjén jelzi a hibát: a Barista Touch ER-kódokat mutat, az Oracle "Error" feliratot, az Oracle Jet E-számokat. A **Dual Boiler BES920** más utat jár. Nála a hibatábla egyszerű kétszámjegyű kódokból áll, **00-tól 12-ig**, és nem a hétköznapi kijelzőn lakik: egy rejtett öntesztmenüben található, amelyhez gombkombináció kell. Normál használat közben sosem látjuk őket — tudni kell, hol keressük.

A számozást érdemes megérteni, mert szép, rendezett tábláról van szó: a kód blokkja megmondja, milyen típusú hibáról van szó, a blokkon belül pedig a kód nevezi meg a panaszkodó alkatrészt.

## A hibanapló kiolvasása

1. Kapcsoljuk ki a gépet a falikapcsolónál.
1. Tartsuk nyomva az **EXIT** és a **MANUAL** gombot, miközben visszakapcsoljuk az áramot; megjelenik az öntesztmenü.
1. A **MENU** gombbal lépjünk a 3. pontra, a hibanaplóra. A 4. pont mutatja a kazánszint állapotát, LLL (alacsony) vagy HHH (magas) formában.
1. A hibanaplóban a **MENU** léptet a 00-tól 12-ig terjedő kódokon, mindegyiknél a tárolt darabszámmal.
1. Az "ErSt" pontnál tartsuk nyomva a **MANUAL** gombot, amíg sípol: ez törli a tárolt kódokat; a csészecszámláló nem nullázódik.

A darabszám legalább annyira beszédes, mint maga a kód. Ami egy éve egyszer előfordult, az történelem; amié hetente nő, az élő, növekvő gond.

## Mit takar a 00-as blokk

A **00–05** kódok a hőérzékelők blokkját adják, három párra szervezve. Minden páron belül az alacsonyabb szám azt jelenti, hogy a vezérlőelektronika **nem észleli** az érzékelőt — nyitott áramkörként olvassa —, a magasabb szám pedig **rövidzárlatot**:

- **00 és 01** — a gőzkazán hőérzékelője: nem észlelhető, majd rövidzár.
- **02 és 03** — a kávékazán hőérzékelője: nem észlelhető, majd rövidzár.
- **04 és 05** — a főzőcsoport fűtésének hőérzékelője: nem észlelhető, majd rövidzár.

A BES920-ban két rozsdamentes kazán és fűtött főzőcsoport dolgozik, így ez a három NTC hőérzékelő fedi a gép három fűtött zónáját. A [00-as kód oldala](https://hu.codefixcoffee.com/breville/dual-boiler-bes920/00/) a gőzkazán-érzékelőt járja körül, de a tanácsa átvihető a másik öt kódra is: mielőtt alkatrészt vennénk, húzzuk le és vizsgáljuk meg az érzékelő csatlakozóját, és figyeljük a nedvességet — a csatlakozón áthidaló víz attól függően olvashatódik nyitott áramkörnek vagy rövidzárnak, hogy épp hogyan áll. Az eredeti NTC hőérzékelő-szerelvények €25–90 közé esnek attól függően, melyik hármasba tartoznak; az O-ring szettek €10–20-osak, és sokszor úgyis ők az igazi ok.

## Gőzoldal és főzőoldal

A tábla hátralévő része ugyanazt a hardveres választóvonalat követi, mint az érzékelőpárok:

- **Gőzkazán:** 06 (szivattyúprobléma induláskor), 07 (vízszint- vagy szivattyúhiba) és 11 (túlmelegedés).
- **Kávékazán — a főző oldal:** 08 (szivattyú- vagy áramlási hiba), 09 (vízszinthiba) és 10 (túlmelegedés).
- **Főzőcsoport:** 12 (túlmelegedés).

### A kódok, amelyek együtt járnak

Ezek a hibák összefüggnek, ezért a teljes naplót érdemes elolvasni, nem csak egyetlen kódot. A 08 azt jelenti, hogy a szivattyú futott, de az áramlásmérő nem látott semmit — leggyakrabban mészkő ül az áramlásmérő lapátján, vagy egy kicsi szivattyú zümmög vízmozgás nélkül, és mindkét esetben az első teendő a mészetlenítés. A 11-es, a gőzkazán túlhő, jellemzően olyankor következik, amikor a kazán nem töltődik vissza — nézzük meg, a 07-nek vagy a 08-nak is van-e darabszáma —, mert a fűtőelem így is melegíti az alacsony kazánt; a másik ok a szonda tömítésének szivárgása. Bármi rendelése előtt nézzük meg az öntesztmenü 4. pontját: ha a szintállapot ellentmond annak, amit töltéskor hallunk, az megmutatja, melyik oldalon van valójában a hiba.

A 12-es, a főzőcsoport túlmelegedése, a tábla ritkább végén ül, és itt számít a legtöbbet a visszatérés gyakorisága — az újra és újra jelentkező túlmeleg inkább a tápegység-lapkán beragadt fűtésre utal, mint érzékelő-eltérésre. A [12-es kód oldala](https://hu.codefixcoffee.com/breville/dual-boiler-bes920/12/) végigmegy rajta.

## Mibe kerülnek az alkatrészek

- Mészetlenítőszer az áramlás- és szintkódokhoz: kb. €10, és a valódi eseteinek egy részét meg is oldja.
- Töltőszivattyú: €30–60.
- Gőzkazán-szonda O-ring szettel: kb. €85; maga az O-ring szett €10–20.
- Hőbiztosíték: €10–20 — de előbb derítsük ki, miért égett ki.
- Triac vagy tápegység-lapka: €80–150.

Garancián kívüli Breville-szerviz belső hibákra jellemzően €300–500-tól felfelé áraz, ezért egy szivattyú vagy egy érzékelő házilag megéri; idősebb gép lapkáját előbb vessük össze egy árajánlattal. A kazán tetején víz és hálózati feszültség ugyanazon a helyen van: szondákhoz nyúlás előtt húzzuk ki a gépet. Ilyen szétszereléshez jó kiindulópontot adnak az [iFixit szerelési és biztonsági útmutatói](https://ifixit.com).

### Sage néven, itthon

Magyarországon ezt a gépet nem Breville-ként találjuk: nálunk a Sage márkanév alatt kapható az európai kereskedelemben — a [Sage Appliances hivatalos oldala](https://sageappliances.co.uk) az európai márka bemutatója —, a gép műszakilag ugyanaz, csak a név más. Alkatrészt és leírást ezért BES920-ként is keressünk, ne csak Sage-ként. És mert a magyar csapvíz kemény, a 08-as kód mögötti mészköves áramlásmérő nálunk gyakoribb ok, mint a gyári átlag: a rendszeres mészetlenítés szinte kötelező.

A tartomány többi gépe hogyan fogalmazza meg a hibáit, azt a [Breville-szekció](https://hu.codefixcoffee.com/breville/) mutatja be — az ER-családos gépek a diagnosztikai gondolatmenetet megosztják vele, a számozást nem.
