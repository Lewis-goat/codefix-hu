---
title: "Breville/Sage Oracle gőz- és ER kódok: ezt nézze meg először"
description: "Gőzoldali hibák a Breville/Sage Oracle gépen: mit jelentenek a gőzoldali Error és ER kódok, és mi az első lépés."
---

A gőzoldal az Oracle legfoglalkozatottabb része: rozsdamentes gőzkazán, automata gőzölésű gőzkar, szintszondák és töltőszivattyú, mind naponta üzemhőfokon — és a gép hibakódjainak jelentős része is innen származik. A gépcsalád egy 32 bejegyzéses, ki nem adott szerviztáblát használ, Nagy-Britanniában pedig ugyanaz a hardver **Sage** jelzéssel fut, azonos kódokkal. Mielőtt meghibásodott alkatrészre gyanakodna, végezze el az olcsó ellenőrzéseket: a gőzoldali leállások többsége eltömődött gőzcsúcsra, elmaradt öblítésre vagy a szondán csapódó mészkőre vezethető vissza.

## Hol ülnek a gőzkódok az Oracle táblában

Az Oracle (BES980) és az Oracle Touch (BES990) közös táblát használ; a BES980 „Error 1”-től „Error 32”-ig számoz, a BES990 ER-előtagot tesz a bejegyzések elé. A gőzoldali kódok öt helyre csoportosulnak:

- **Error 1–4** — a gőzkazán hőérzékelője: induláskori nyitott kör, üzem közbeni megszakadás, és a két rövidzárlatos eset. Egy érzékelő, négyféle jelentés.
- **Error 13–16** — ugyanez a négyes a gőzkar saját hőérzékelőjén, azon a szondán, amely a megfelelő tejhőmérséklet elérésénél leállítja az automata gőzölést. A gép legvizesebb pontján lakik.
- **Error 18** — a gőzkazán nem melegszik fel rendesen.
- **Error 20 és 21** — gőzkazán-vízszint- vagy töltőszivattyú-probléma, illetve a szintszonda a vezérlőelektronika által várttal ellentétes értéket ad.
- **Error 26** — a gőzkazán a célhőfok fölé melegedett; **Error 32** — gőzkazán-szivárgás vagy sikertelen újratöltés.

Nem minden, a gőzkar közelében keletkező kód gőzoldali: az 5–8 a kávékazán érzékelőjéhez tartozik, köztük a [Error 8](https://hu.codefixcoffee.com/breville/oracle-bes980/error-8/), az üzem közbeni rövidzárlat bejegyzésével. A tárolt napló segít szétválasztani a családokat — BES980-nál a kikapcsolt gépen tartott 1 CUP + 2 CUP + POWER kombináció nyitja meg az Error Storage-t, ahol mind a 32 kód végigléptethető a számlálóival.

## Először ezt nézze meg: a gőzkar öblítése

A gyenge, köpködő gőz vagy egy kód közvetlenül tejes ital után inkább a gőzcsúcsra, mint a kazánra mutat:

1. Húzza ki a gépet, és várja meg, amíg a gőzkar kihűl.
1. Csavarozza le a gőzcsúcsot, áztassa forró vízben kevés mészetlenítő szerrel, és a tisztítótűvel járja át minden lyukát.
1. Futtassa le az öblítést: körülbelül tíz másodperc gőz a cseppgyűjtőbe, csúcs nélkül, majd még egyszer a csúccsal együtt.
1. Mostantól minden tejes ital után öblítsen: a csúcsban megszáradt tej indítja a legtöbb ilyen leállást.

Ha a gép figyeli a gőznyomást, ahogy az Oracle Jet teszi az E16 kóddal, egy kéregszerű csúcs már akkor hibakódot dob, mielőtt észrevenné, hogy legyengült a gőz.

## Keménység, mészkő és a szintszondák

Kemény víznél a mészkő maga írja a hibakódokat. A gőzkazán szintszondái állandóan forró vízben állnak, a rájuk csapódó mészkéreg pedig szigetel — a vezérlőelektronika így akkor is „nincs víz” jelzést olvas, ha a kazán valójában tele van. Ez a klasszikus út az Error 20 vagy 21 felé, és az Error 32 újratöltési hibája is ide fut be. A mészkő a gőz útjában és a töltőszivattyú szűrőjén is felhalmozódik. Egy teljes mészetlenítés, a gőzkazán-körrel együtt, a legolcsóbb diagnosztika, és meglepően sok kódot magától eltüntet; a helyes elvégzésben a [Sage támogatási oldala](https://sageappliances.co.uk) részletes útmutatókkal segít.

A paletta testvérgépe is ugyanezt a leckét mondja el: a Dual Boiler a 00–12 kódjait rejtett önteszt menüben őrzi, és a [00-s kód](https://hu.codefixcoffee.com/breville/dual-boiler-bes920/00/) — a gőzkazán-érzékelő nem észlelhető — egy olyan tábla tetején ül, amelynek szint- és töltésbejegyzései kemény víz mellett pontosan ugyanígy viselkednek.

## Mikor elég a mészetlenítés, és mikor kell szétszerelni

Előbb mészetlenítés, utána szétszerelés — de érdemes tudni, hol ér véget a mészetlenítés haszna:

- **Mészetlenítsen először** a szint-, szonda- és újratöltési kódokra (20, 21, 32), a kód nélküli gyenge gőzre, és minden gépen, amelyet utoljára több mint három hónapja mészetlenítettek. Költség: egy üveg mészetlenítő szer.
- **A mészetlenítés nem segít** azokon az érzékelőkódokon, amelyek frissen mészetlenített, bemelegedett gépen azonnal visszatérnek — legyen szó a gőzkazán 1–4 közüli bejegyzéséről vagy a kávéoldali [Error 8](https://hu.codefixcoffee.com/breville/oracle-bes980/error-8/)-ról. A mészetlenítést túlélő kód az érzékelőre, annak kábelére vagy egy csatlakozóra mutat.
- **Álljon meg a tömítéseknél**, ha az Error 26 ismétlődik: a szivárgó gőzszonda-O-gyűrű hagyja, hogy a gőz felmelegítse az érzékelő kábelét, és kiszaladt kazánnak tetteti magát. Az új szonda-O-gyűrű olcsó; egy triac, amely nem kapcsolja ki a fűtést, nem az.
- **Error 18** egy gépnél, amelyik egyáltalán nem ad már gőzt, jellemzően fűtésoldali ok — hőbiztosíték, fűtőelem vagy elektronika —, nem mészkő, tehát javítási és nem tisztítási ügy.

## Mibe kerülnek az alkatrészek

A gyári hőérzékelő-szerelvények €25–€95 közé esnek, a szonda személyétől függően; a gőzkarszerelvények, érzékelőjükkel együtt, €60–€95 körül mozognak; egy szonda- és O-gyűrűs szett kb. €85, a töltőszivattyú €30–€60. Ezzel szemben a garancián kívüli gyári ajánlatok belső hibákra jellemzően €300–€500 — az „előbb egy üveg mészetlenítő, utána érzékelőszintű javítás” sorrend ezért szinte mindig jobb üzlet. A Sage-feliratú változatok lefedettségét a [webhely brit kiadásán](https://hu.codefixcoffee.com/uk/) találja.

### Vízkeménység itthon

Magyarországon a csapvíz nagy területeken közepesen kemény vagy kemény, így az Oracle gőzkazánában a mészkő gyorsabban felépül, mint a gyári alapidőközök sugallják. A helyi vízmű honlapján utánanézhet a környéke keménységének, és ehhez igazíthatja a mészetlenítés gyakoriságát. Sok háztartásban a palackos vagy szűrt, lágyabb vízzel való üzemeltetés bizonyul a legjobb kompromisszumnak az íz és a gép élettartama között.
