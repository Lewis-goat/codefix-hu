---
title: "Jura Error 6 és 7: a kerámiaszelep, őszintén elmondva"
description: "A Jura Error 6 és 7 a motoros kerámiaszelepet jelzi: mészetlenítés, tömítés vagy jeladó? Miért lesz az Error 7-ből jellemzően műhelymunka."
---

A Jura számozott hibakódjai megnyugtatóan konkrétak. Az Error 1–5 a termoblokk-fűtőkre és azok hőérzékelőire, a 8 a főzőegységre, a 12 a darálóra mutat. A 6 és a 7 viszont ugyanarról az alkatrészről szól: az elektronikus kerámiaszelepről, a motorosan forgatott korongról, amely a gép belsejében útvonalakra tereli a vizet. A két kód közti különbség nagyjából annyi, mint a „futtass le egy mészetlenítést és nézd meg" és a „foglalj műhelyidőt" közti. Íme, mi zajlik a háttérben.

## Mivel foglalkozik a kerámiaszelep?

A legtöbb bean-to-cup gép egyszerű mágnesszelepekkel vált kávé, forróvíz és gőz között. A magasabban felszerelt Jurák — a Z5-től a Z10-ig, az X széria, a J5–J9, a GIGA sor és az újabb S és E modellek — helyette elektronikus kerámiaszelepet használnak: egy kis motor pozíciók között forgat egy kerámia korongot, a korong csatornái pedig a kifolyóhoz, a forróvíz-csaphoz vagy a gőzkörhöz irányítják a vizet. Egy pozíciójeladó (encóder) minden pillanatban jelzi, hol tart a korong, így a vezérlőelektronika biztos lehet benne, oda megy-e a víz, ahová szánta.

Ez a visszajelzési kör magyarázza, hogy egyáltalán létezik Error 6 és 7: az elektronika pozíciót parancsol, megvárja az encóder visszaigazolását, és hibát ír ki, ha az elmarad.

## Error 6: a korong nem ért oda

Az [Error 6](https://hu.codefixcoffee.com/jura/automatic-machines/error-6/) jelentése, hogy a kerámiaszelep nem működik rendesen: a korong nem érte el azt a pozíciót, amelyet a vezérlőelektronika kért tőle. A gyakorlatban három ok jöhet szóba, valószínűségi sorrendben. A mészkeményedés megmerevíti a mechanikát, és a motor nem tudja szabadon forgatni a korongot. A szivárgó tömítés vizet enged a hajtásba, nedvesítve a motort és az encódert. Vagy maga a motor, illetve a jeladó hibásodott meg. A legvalószínűbb ok ingyen javítható — kezdd ott.

1. Futtass le először egy teljes mészetlenítési ciklust. A merev kerámia korong első számú oka a mészkeményedés, a megoldás pedig egy tabletta és egy óra.
2. Indítsd újra a gépet, és hallgasd. Induláskor a szelep hallható kattogással végigfut a pozícióin; ha az indító ciklus most teljesen lefut, kész vagy.
3. Ha az Error 6 megmarad, a gépet fel kell nyitni: nézd meg, nincs-e víz a szelepház körül. A nedvesség arra utal, hogy szivárgó tömítés szennyezi a hajtást.
4. A javítás maga a szelep tisztítása vagy cseréje. A motort és a szelepet szabály szerint egyetlen egységként cserélik, nem külön-külön.

Kerámiaszelep-egységre kb. 55–110 €-val számolj; ha csak a tömítéskészlet kell, 10–18 €-tal.

### Hazai tipp: a mészetlenítés nálunk nem opció

Magyarországon a vezetékes víz keménysége az ország nagy részén magas, így a kerámiaszelep pont az az alkatrész, amelyet a mészkeményedés elsőként megtámad. Használj a vízkeménységhez igazított szűrőpatront, és tartsd be a gép mészetlenítési jelzéseit — a sorra kihagyott mészetlenítések a drága szelepcsere leggyakoribb előzményei. Eredeti tablettát a [Jura hivatalos honlapján](https://www.jura.com) található kereskedőkeresővel és hazai forgalmazóknál is vegyél.

## Error 7: a komoly testvér

Az [Error 7](https://hu.codefixcoffee.com/jura/automatic-machines/error-7/) ugyanazt a hardvert éri sokkal keményebb csapáson, a főzőegység-hajtással kiegészítve: a gép a kerámiaszelepet (GIGA modelleken a többfunkciós szelepet) pozícióba parancsolta, és a visszaigazolás sosem érkezett meg, vagy közben a főzőegység-hajtás viselkedett rosszul. A GIGA X3c-n és X8c-n konkrétan a hibás többfunkciós szelepet jelzi, a GIGA 6-on pedig gyakran motor- vagy pumpablokádként jelentkezik. Ez az egyik kevés Jura kód, amelyhez nincs megbízható felhasználói szintű megoldás.

Ez nem jelenti, hogy a foglalás előtt semmi értelme próbálkozni.

1. Húzd ki a gépet öt percre, majd indítsd újra. Az indítási ciklus alaphelyzetbe állítja a főzőegységet és a szelepet is, így egy átmeneti akadás magától is tisztulhat.
2. Zárd ki az olcsó okokat: ürítsd ki a kávéüledék-tartályt és a csöpögtetőtálcát, győződj meg róla, hogy nincs beszorulva semmi a kifolyóban, és futtass le egy teljes tisztítóprogramot megszakítás nélkül.
3. Ha a kód ezek után is visszatér, a szokásos belső lelet maga a szelep-egység: repedt kerámia korong, beragadt működtető vagy elromlott pozíciójeladó.

## Miért műhelymunka az Error 7?

Ennél a kódnál az őszinte tanács: műhelypad, hacsak nem foglalkozol amúgy is ilyen gépek szervizelésével. Az okok praktikusak, nem titokzatosak.

- A Jura házakat biztonsági (ovális fejű Torx-Plus) csavarok tartják, és a hálózati feszültség közel dolgozik az ember keze.
- A gépből a vizet teljesen le kell ereszteni, mielőtt a szelephez nyúlnál, és maga a szerelés is aprólékos munka.
- Szelep- vagy főzőegység-motorcsere után a mechanizmust újra kell kalibrálni, különben a vezérlőelektronika nem bízhat meg a pozíciójelekben.

Az alkatrészek legtöbb modellhez léteznek — kerámia- vagy többfunkciós szelep-egység modelltől függően kb. 55–140 €, főzőegység-motor 40–65 € —, a munkadíj viszont jellemzően magasabb az alkatrésznél, ezért kérj árajánlatot, mielőtt bármit rendelsz. A garancián kívüli gyári szerviz szuperautomatáknál jellemzően 230–460 € közé esik a visszaszállítással együtt; a független kávégépszervizek — itthon is több működik belőlük — egy jól körülírt alkatrészcsere esetén általában olcsóbbak.

## Megéri-e javíttatni?

A kerámiaszelepes Jurák többnyire éppen az a kategória, amit érdemes megtartani; egy mészetlenítéssel elmúlt Error 6 nem került semmibe. A 7-esnél a számítás modellfüggő: egy csúcsmodell Z-n vagy GIGA-n a javítás általában megtérül, egy tízéves belépő szintű E-n vagy ENA-n viszont az árajánlatot érdemes egy felújított géppel szemben is mérlegelni.

Nem minden Jura kód végződik műhelyben. Az [Error 12](https://hu.codefixcoffee.com/jura/automatic-machines/error-12/) — a klasszikus, kővel beragadt daráló — jellemzően porszívóval és a babok átvizsgálásával megoldható. A teljes lista, a termoblokk- és főzőegység-kódokkal együtt, a [Jura hibakód-mutatóban](https://hu.codefixcoffee.com/jura/) található.
