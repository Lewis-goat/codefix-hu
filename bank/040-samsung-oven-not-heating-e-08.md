---
title: Samsung sütő nem melegszik: E-08 és társai
description: Samsung sütő nem melegszik, E-08 hiba? Megszakító, fűtőelem, hőérzékelő, relé — és az ajtózár-változat ellenőrzése sorrendben.
---

Az a sütő, amely bekapcsol, de hideg marad, meglepően jól körülírt módon hibázik: a vezérlés hőfokot állított be, a sütőtér hőmérséklete nem emelkedett, és a gép eltárolta az okot. Samsung tűzhelyeknél és beépített sütőknél erre az [E-08](https://hu.codefixcoffee.com/samsung/range-wall-oven/e-08/) a fő kód — a sütő nem melegszik, és a gyanúsítottak a sütő- vagy grillfűtőelem, a hőérzékelő szonda vagy a vezérlőn ülő relé. Körülötte egy kisebb kódcsalád pontosítja tovább a hibát. Ez a bejegyzés abban a sorrendben vezeti végig őket, amelyben érdemes ellenőrizni — kezdve azzal a lépéssel, amit mindenki kihagy.

## Először: a megszakítós áramtalanítás

Mielőtt bármit is lezárnánk magunkban, kapcsoljuk ki a megszakítónál három percre, majd vissza. Ez nem babona — a rossz állapotba került tűzhely-vezérlés olyan fűtési hibát is naplózhat, amit normál esetben nem tenne, és a tiszta újraindítás ezt törli. Ha a következő sütésnél visszajön az E-08, a hiba valódi, és jöhet a következő lépés. Ugyanez a háromperces reset nyitja meg az utat a [Samsung sütőkód-lista](https://hu.codefixcoffee.com/samsung-oven-error-codes/) csaknem minden kódjánál, tehát megéri megszokni.

## A fűtőelem

Az alsó sütőfűtőelem a sütőtér aljának munkagépe, és látványosan hibázik. Bekapcsolt sütőnél az elemnek a teljes hosszában egyenletesen kell izzania. Látható törés, hólyag vagy égett folt önmagában diagnózis: csere. A fűtőelem €30–60, és a legjobban megérő sütőjavítások közé tartozik. Ha szépen izzik, de a sütő mégsem tartja a hőfokot, az elem fel van mentve, és jöhet a szonda — a teljes döntési út az [E-08 diagnosztikai oldalán](https://hu.codefixcoffee.com/samsung/range-wall-oven/e-08/) található.

## A hőérzékelő szonda

A szonda méri a sütőtér hőmérsékletét, és ellenállásértékként jelzi vissza a vezérlőelektronikának. Szobahőmérsékleten az egészséges szonda kb. 1080 ohmot ad — és ez az érték maga a teszt:

1. Áramtalanítsunk a megszakítónál.
1. Csavarozzuk ki a szondát a sütőtér hátfalából (két csavar), és húzzuk le a dugaszát.
1. Mérjük meg: szobahőn kb. 1080 ohm az egészséges érték.
1. Ha az érték rendben, ültessük vissza a csatlakozót; ha messze esik tőle, cseréljük a szondát.

Két rokon kód multiméter nélkül is elárulja, merre hibázott a szonda. Az E-27 nyitott áramkört jelent — az ellenállás túl nagy, kb. 2950 ohm felett —, vagyis hibás szondát vagy laza dugaszt. Az E-28 rövidzárlatot, kb. 930 ohm alatt, vagyis zárt szondát vagy a sütő mögött beszorult, megnyomódott kábelt. A szonda maga €20–40, és a sütőtérből csavarozható.

## A relé a vezérlőn

Ha az elem izzik, és a szonda is jó értéket mér, a relé táblája marad hátra: a vezérlőelektronika nem kapcsolja rá az elemet a hálózatra. A soha be nem záró relé a sütőn belülről pontosan úgy néz ki, mint egy halott fűtőelem. Ez a €100–200-as kimenet, és idősebb tűzhelynél itt válik ésszerűvé a javítási árajánlat összevetése a gép értékével.

## Az ajtózár-változat

Egy fontos kitétel, mielőtt alkatrészt rendelünk: egyes modelleknél a Samsung saját támogatási oldala az E-08-at ajtózár-hibaként sorolja fel, nem fűtési hibaként — vagyis az öntisztításhoz használt motoros zárra gondol, nem a sütőáramkörre. Az elem megrendelése előtt nézzük meg a saját modellünk kézikönyvét. A zár rokon kódja az E-0E (E-0E-ként vagy FL-ként jelenik meg), amely jellemzően öntisztítási ciklus után jelentkezik, amikor a zár kapcsolója beragad vagy a zármotor tönkremegy; a szerelvény €40–90. Egyik esetben se erőltessük az ajtót — várjuk meg, míg a sütő teljesen kihűl, mert forrón úgysem nyit.

## Az ellenkező irányú baj: E-0A

Már itt tartva érdemes ismerni az [E-0A-t](https://hu.codefixcoffee.com/samsung/range-wall-oven/e-0a/): a sütő túlmelegedését. Más panasznak hangzik, de két gyanúsítottat megoszt az E-08-cal — rosszul olvasó hőérzékelőt (ezúttal aluljelentőt) vagy beragadt, be nem nyitó relét, amely nem kapcsolja le az elemet. Az E-0A-t sürgősebben kell venni, mint a nem-melegszik hibát: a beragadt relé azt jelenti, hogy az elem bekapcsolva marad, ezért azonnal kapcsoljuk ki a megszakítót, és ne használjuk a sütőt, míg meg nem javították.

## Mibe kerül?

- Fűtőelem: €30–60.
- Hőérzékelő szonda: €20–40.
- Ajtózárszerelvény: €40–90.
- Relés vezérlőlapka: €100–200.

Az elem és a szonda bármilyen ésszerű gépkornál egyértelműen megéri; a lapka döntés kérdése. A kiszálló technikus €120–250-ért diagnosztizál, plusz az alkatrész — ez tisztességes ár annak eldöntéséért, hogy a három közül melyikre van valójában szükség.

### Magyarországi gyakorlat

A [Samsung támogatási oldala](https://samsung.com/hu/support/) a típuskód megadásával előhozza a gépünkhöz tartozó dokumentumokat — ez az ajtózár-változat eldöntéséhez különösen hasznos, mert az E-08 jelentése modellfüggő lehet. Garancián belüli sütőnél a szétszerelést bízzuk márkaszervizre, mert az önjavítás a jótállást kockáztatja. Áramtalanításkor pedig emlékezzünk rá: a magyar kapcsolószekrényben a sütő jellemzően saját megszakítóval futó áramkörön ül — azt kapcsoljuk ki, ne csak a gépkapcsolót.
