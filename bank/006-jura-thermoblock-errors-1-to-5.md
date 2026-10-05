---
title: "Jura Error 1–5: a termoblokk-család magyarázata"
description: "A Jura Error 1–5 kódok mind a termoblokkokhoz, az NTC hőérzékelőkhöz vagy a hőbiztosítékokhoz vezetnek vissza. Kódonkénti bontás és az Error 2 csapdája."
---

Az 1-től 5-ig számozott Jura hibakódok elsőre véletlenszerű számhalmaznak tűnnek, közös témájuk mégis egy van: a hő. Mindegyik a termoblokkokra — a kompakt, átfolyós fűtőkre, amelyek a főzővizet és a gőzt előállítják — vagy az őket felügyelő hőérzékelőkre és hőbiztosítékos zsinórokra vezethető vissza. Ha egyszer átlátod a rendszert, egyetlen kód megmondja, melyik fűtő elégedetlen, és hogy a gond mérés, hőmérséklet vagy áramellátás.

## Két fűtő, öt kód

A Jura gépekben két termoblokk dolgozik. A kávés termoblokk a főzővizet melegíti, a gőzös termoblokk pedig a gőz- és forróvíz-oldalt táplálja. Mindegyiken ül egy NTC hőérzékelő — egy olyan ellenállás, amelynek értéke a hőmérséklettel változik, és a vezérlőelektronikának jelent —, mindkettőt pedig hőbiztosítékos zsinórok védik, amelyek túlzott melegedésnél megszakítják az áramot. Az Error 1–5 az elektronika módja, hogy közölje: ezek az elemek egyike rosszul van.

- **Error 1 és 2** a kávés termoblokk hőérzékelő-körére mutat.
- **Error 3 és 4** a gőzös termoblokkra — túl alacsony jelzés, illetve túlmelegedés.
- **Error 5** pedig maga a fűtőelem, amely nem teljesít.

## A kávé oldala

### Error 1: kávés termoblokk-hőérzékelő hiba

Az [Error 1](https://hu.codefixcoffee.com/jura/automatic-machines/error-1/) azt jelenti, hogy a vezérlőelektronika nem kap értelmes jelzést a kávés termoblokk hőérzékelőjéről — az S, X, J és Z családokon ez a klasszikus hőérzékelő-hiba, az F-n és az E80-nál jellemzően sérült hőérzékelő áll mögötte. Egy apró csavar a rendszerben: a hideg autóból vagy garázsból frissen behozott gép ép alkatrészekkel is kódolhat így. Ha meleg gépen jelenik meg, és újraindítás után azonnal visszatér, a hőérzékelő-kör megszakadt — maga a hőérzékelő, a kábele vagy a blokkot tápláló hőbiztosítékos zsinórok.

### Error 2: megszakadt jel — vagy csak hideg a gép

Az [Error 2](https://hu.codefixcoffee.com/jura/automatic-machines/error-2/) minden Jura-kód közül a leggyakoribb, és kétarcú természetű. A jóindulatú változat: a gép kb. 10 °C alatt van, és a fűtő szándékosan zárolva van, amíg fel nem melegszik — télen szállított vagy hideg helyiségben tartott gépeknél gyakori. A komoly változat: a kávés termoblokk hőérzékelője vagy a hőbiztosítékos zsinórok megszakadtak.

Éppen ezért a felmelegítés a diagnózis. Hozd a gépet szobahőre — sok tulajdonos alacsony fokozatú hajszárítóval öt percre a víztartály üregébe fújva melegít, vagy langyos (nem forró) vízzel töltött tartállyal segít —, majd indítsd újra. Ha a kód eltűnik, semmi sem tört el, csak tartsd melegebb helyen a gépet. Ha meleg gépen is megmarad, a hőérzékelő-kör nyitott, és az NTC hőérzékelő valamint a biztosítékzsinórok belülről ellenőrzendők.

### Hazai tipp: a téli éléskamra-csapda

Magyarországon sok háztartásban a kávégép nem a fűtött konyhában, hanem kamrában, nyaralóban vagy hétvégi házban telel, ahol télen akár 10 °C alá is süllyed a hőmérséklet — pontosan az Error 2 jóindulatú változatának feltétele. Mielőtt szerelőt hívnál, vidd a gépet egy meleg szobába, hagyd ott néhány órát, és csak ezután indítsd újra. A hazai vezetékes víz ráadásul nagy területeken kemény, így a mészetlenítést se halogasd: a mészkeményedés az Error 3 és 4 rendszeres előszobása.

## A gőz oldala

### Error 3: a gőzös termoblokk alacsonyat mutat

Az [Error 3](https://hu.codefixcoffee.com/jura/automatic-machines/error-3/) az Error 1 gőz-oldali tükörképe: a gőzös termoblokk nem jelent hőmérsékletet — a hőérzékelő, a kábel vagy a még mindig túl hideg gép miatt. Egy további szempont: az erős mészkeményedés annyira lelassíthatja a felfűtést, hogy egyes firmware-eken a hőfok-ellenőrzés elbukik, ezért szétszerelés előtt egy teljes mészetlenítés is feltétlenül a teendők közé való. Belül a hőérzékelő-kábelt ott érdemes megnézni, ahol hajlik.

### Error 4: a gőzös termoblokk túlmelegszik

Az [Error 4](https://hu.codefixcoffee.com/jura/automatic-machines/error-4/) a komolyan veendő tagja a családnak. A gőzös termoblokk a vártnál magasabb hőfokra futott fel — vagy a hőérzékelő mutat kevesebbet a valósagnál (mészkeményedés szigeteli, korrodált érintkezők), vagy a tápegység-elektronika nem szakította meg a fűtést. A Jura szerint az Error 2 mellett ez a két leggyakoribb javítás. Lehűlés és mészetlenítés után az első csere a hőérzékelő; ha új NTC hőérzékelővel is újra túlmelegszik a blokk, a tápegység nem kapcsolja ki a fűtőelemet, és cserélni kell — számolj 120–250 €-val. Az örökké égő fűtő tűzveszély: amíg ez a kód él, ne hagyd a gépet felügyelet nélkül bedugva.

### Error 5: a fűtő nem éri el a hőfokot

Az [Error 5](https://hu.codefixcoffee.com/jura/automatic-machines/error-5/) azt jelenti, hogy a fűtőelem megkapta a parancsot, a hőmérséklet mégsem emelkedett. Jura gépen ez szinte mindig a termoblokkot védő hőbiztosítékos zsinórok — amelyek túlmelegedés után vagy egyszerű öregedéssel égnek el —, a másik lehetőség a halott termoblokk-fűtőelem. A nagyon hideg gép szintén okozhatja, ezért először melegítsd fel. Belül mérd meg mindkét biztosítékzsinórt és a fűtőelemet: amelyik megszakadtat mutat, az a cserélendő alkatrész — utána pedig derítsd ki, miért égtek el a biztosítékok (mészkeményedés, beragadt relé vagy szárazüzem, amikor a tartály kifogyott).

## Ami a családot összeköti

Ebben a családban a hőbiztosítékos zsinórok és az NTC hőérzékelők a visszatérő szereplők — egy eredeti Jura NTC kb. 25–40 €, egy biztosítékzsinór-szett 15–30 €, egy termoblokk pedig 90–180 €. Hőérzékelőcserekor a szakmai gyakorlat a biztosítékzsinórok együttes cseréje. És egy minta, amit érdemes észben tartani: a néhány napon belül újra elégő biztosítékzsinór nem peches új alkatrészt jelent, hanem azt, hogy a tápegység ragadja be a fűtőt.

Jó tudni, hogy a Jura házak biztonsági csavarokat használnak, a termoblokkokon pedig hálózati feszültség van — ez a család megfelelő felszerelés nélkül műhelymunka. S, Z, GIGA és újabb E-sorozatú gépeken megéri javíttatni; egy tízéves Impressánál viszont az árajánlatot mérlegeld egy felújított gép árával. A modellspecifikus gyári adatokhoz a [Jura hivatalos honlapja](https://www.jura.com), a többi kód kontextusához a [Jura hibakód-mutató](https://hu.codefixcoffee.com/jura/) a kiindulópont.
