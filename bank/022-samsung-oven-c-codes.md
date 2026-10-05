---
title: "Samsung sütő C-kódok: az okos tűzhelyek hőmérséklet-családja"
description: "Samsung C-21, C-24, C-F2: túlmelegedési leállás, gyors hőemelkedés a szellőzésnél, hűtőventillátor-hiba NE és NX tűzhelyeken, árakkal."
---

A Samsung tűzhelyek és beépített sütők — az NE- és NX-szériák, illetve NV és NZ testvéreik — két dialektusban beszélnek. A kéttagú kódok (például E-08, E-27) a sütő fűtőelemeiről szólnak, a rövid kódok (SE, tE) a kezelőpanelról. Kettejük között helyezkedik el a C-család — C-21, C-24 és C-F2 —, a hőmérséklet- és ventilátorfelügyelet kódjai, amelyeket a [Samsung sütő kódindexünk](https://hu.codefixcoffee.com/samsung-oven-error-codes/) gyűjt egy helyre. Ez a hármas érdemli a legnagyobb figyelmet, mert legalább egyik tagja azt jelzi, hogy a sütő valóban túlmelegedett.

## Nincs kiolvasható hibanapló

Samsung sütőben nincs a felhasználó számára elérhető hibanapló. A kód addig ül a kijelzőn, amíg meg nem szűnik az ok, vagy amíg ki nem kapcsolja a gépet az automata megszakítóról — a C-kódos eljárások öt-tíz perc szünetet írnak elő —, és ha a visszaállítás után újra jelentkezik, vegye valós hibának, ne a folyamatos resetelésben reménykedjék.

## C-21: a túlmelegedési leállás

A [C-21](https://hu.codefixcoffee.com/samsung/range-wall-oven/c-21/) a biztonsági felügyelet jelentése: a sütőkamra hőmérséklete a megengedett sáv fölé kúszott, ezért a vezérlőelektronika leállította a fűtést. Több tulajdonos is arról számolt be, hogy a tűzhely a kód megjelenése előtt veszélyesen felforrósodott — a C-21 tehát azonnali állj-jel a főzéshez, nem kellemetlen csörgés. A leggyakoribb gyanúsított a kamra hőmérséklet-érzékelője a vezetékezésével együtt; a fő nyomtatott áramkör a második a listán.

1. Kapcsolja ki az automata megszakítóról öt-tíz percre, és egyszer tesztelje újra: ha a következő felfűtéskor visszatér a C-21, a hiba valós.
1. Áramtalanítás után szerelje ki a kamra hátfalán ülő érzékelőszondát rögzítő két csavart, és húzza elő a csatlakozót a vezetékezéssel.
1. Mérje meg a szondát multiméterrel: szobahőmérsékleten kb. 1080 Ω az egészséges érték; szakadt vagy eszeveszett olvasás esetén cserélje.
1. Nézze meg a csatlakozó dugházát hőkárosodás után ott, ahol a fűtőelem közelében halad — egy megolvadt csatlakozó ugyanezt a kódot produkálja.
1. Ha az érzékelő jó, és a hiba akkor is kiold, a vezérlőelektronika szabályozza rosszul a fűtőelemeket: ez már szervizszintű javítás.

## C-24: a gyors hőemelkedés ellenőrzése

A [C-24](https://hu.codefixcoffee.com/samsung/range-wall-oven/c-24/) a szellőzés és a vezérlés környékén jelentkezik: az elektronikatér gyorsabban melegszik, mint amit a vezérlőelektronika vár. A Samsung a C-24/C-25 családot a szellőztető zónához kötött fűtési túlhőjelként dokumentálja; a gyakorlatban az ok háromfelé ágazik: soha be nem pörgő hűtőventillátor, a tűzhely körül elzárt légáramlás vagy egy haldokló túlhő-termisztor, amely egészséges területet forrónak érzékel.

A diagnózis főleg hallásra és látásra megy. Reseteljen a megszakítóról, indítson sütési programot, és füleljen, hallatszik-e a konvektor- és a hűtőventillátor, ahogy a gép melegszik — a csend maga a válasz. Ellenőrizze a beépítési hézagokat, és azt, hogy a tűzhely alatt vagy mögött nem tömik-e el a szellőzőnyílásokat bútor, fólia vagy por. Áramtalanítva a túlhő-érzékelő (NTC hőérzékelő) a csatlakozójánál lemérhető — ugyanabba a kb. 1000 Ω-os osztályba esik, mint a kamraszonda, a szakadt vagy vándorló olvasást adót cserélni kell. Ha a ventilátor halott, cserélje ki, mielőtt a vezérlőelektronika szétfőzi magát: a hő az ok, a panel az áldozat.

## C-F2: a hűtőventillátor visszajelzése

A [C-F2](https://hu.codefixcoffee.com/samsung/range-wall-oven/c-f2/) túlmelegedés-kódnak tűnik, de jellemzően nem az. A C-F család azt jelenti, hogy egy felügyelt alkatrész nem válaszol a vezérlésnek, C-F2-nél pedig ez a hűtőventillátor-kör: a kijelzőelektronika nem kapja meg a várt visszajelzést. Vagy a ventilátor tényleg nem forog, vagy a csatlakozója lazult ki vagy perzselődött be, vagy a panel felé menő jelvonal szakadt meg.

Menjen végig rajta sorban. Megszakítós reset után fűtse fel a sütőt, és nézze meg, forog-e fizikailag a ventilátor. Forgó ventilátor mellett a visszajelzési útra gyanakodjon: ültesse vissza a panelen a ventilátor csatlakozóját, és keresse a hő miatti elszíneződést a tűkön. Néma ventilátornál először beragadt lapátot keressen — por, vagy a panel mögé hullott csavar —, majd mérje meg a tekercset szakadásra. A ventilátor- és csatlakozójavítás olcsó; a mindkét próbán átment C-F2 már a fő panel bemenetére mutat.

## Mennyibe kerülnek az alkatrészek

A kamra hőmérséklet-érzékelő €15–€40, és tízperces csavarozós munka — a család leggyakoribb javítása. A hűtőventillátor €40–€90, a kábelkészletek €10–€20. A drága tétel a fő vezérlőelektronika, €150–€300, és arra csak akkor gondoljon, ha az érzékelő és a ventilátor már kizárva. A szerelői kiszállás diagnózissal és alkatrésszel együtt kb. €120–€250; garancián kívüli, panelhibás gépnél előbb kérjen árajánlatot, és csak utána rendeljen bármit. Ha szerelőhöz fordulna, a [Samsung magyar honlapján](https://www.samsung.com/hu/) is talál támogatási kapcsolatot.

Egy szabály az egész családra érvényes: ne resetelgesesse a C-21-et, és ne folytassa mellette a sütést. A kód azt jelenti, hogy a vezérlőelektronika már látott egy neki nem tetsző hőfokot — a következő kioldás a skála magasabb pontján következhet be.

### Magyarországi beépítés: megszakító és hézagok

Magyar konyhákban a beépített sütőket jellemzően nem dugaszra, hanem fix bekötéssel szerelik, így a „kapcsolja ki a fali aljzatról” lépések helyett a lakáselosztó megfelelő automata megszakítóját kell kikapcsolnia. A beépítéskor a kézikönyv előírta szellőztető hézagokat gyakran szűkíti a bútorzat vagy a sütő alá gyömöszölt tepsik, sütőlemezek — pont azt a légáramlást zárják el, amelyet a C-24 jelez. Évente egyszer húzza ki a gépet, és tisztítsa fel a környékét, mielőtt a por és a zsír összereged.
