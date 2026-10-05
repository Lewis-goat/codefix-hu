---
title: "Jura Error 12: kavics akadt a darálóban"
description: "A Jura Error 12 azt jelzi, hogy a daráló nem forog — jellemzően kavics szorult a korongok közé. Így távolítható el az akadály."
---

Amikor egy Jura kijelzőjén Error 12 jelenik meg, a hiba oka szó szerint kézzel fogható: valami olyan került a babok közé, ami oda nem való. A vezérlőelektronika kiadta az őrlési parancsot, a daráló mégsem mozdult. Két darálós GIGA gépeken a kód kifejezetten a bal oldali darálót nevezi meg. A gyakorlatban a kiváltó ok szinte mindig idegen tárgy — klasszikusan egy apró, betakarításkor a babok közé keveredett kavics —, amely a darálókorongok közé ékelődik. A részleteket a [teljes Error 12 referencia](https://hu.codefixcoffee.com/jura/automatic-machines/error-12/) tartalmazza; ez a bejegyzés arról szól, hogyan juthatunk hozzá az akadályhoz, és mikor merül fel, hogy a hiba sokkal több egy kavicsnál.

## Mit mond valójában a kód

A Jura az E, ENA, S, J, Z és GIGA sorozatokban közös, számozott hibalistát használ, és a 12-es a darálóhoz tartozik: a motor beragadt, vagy a korongok nem tudnak szabadon fordulni. A súlyosság közepes, a javítás mérsékelten barkácsolóbarát — több, mint egy cseppgyűjtő kiürítése, de ha tényleg beszorulásról van szó, és nem elhalt motorról, a ház felnyitása nélkül is gyógyítható.

A GIGA-kérdés pedig számít: ezekben a gépekben két daráló dolgozik, és az Error 12 a **bal** oldalit jelöli, így nem találgatni kell, melyiket vizsgáld meg először.

## A szokásos tettes: kavics a babban

A kávé mezőgazdasági termék: előfordul, hogy egy apró kavics túléli a betakarítást és a válogatást, és bekerül egy zsák babba. Ami elég kicsi ahhoz, hogy átcsússzon az adagoló kifolyóján, pontosan akkora, hogy a két korong közé ékelődjön — a daráló az első érintkezésnél megáll. A sötét pörköletből időnként kialakuló, összetapadt darabkák ugyanígy gátolhatják a mechanizmust. Mindkét esetben a hiba mechanikai, nem elektronikai: nem a vezérlőelektronikával van baj, hanem ki kell szedni az akadályt.

## A második ok: az olajos finomságokra beragadt motor

A másik dokumentált ok látványtalanabb, de többe kerül. Az öreg, olajos kávéfinomságok — a porszerű szemcsék, amelyeket a sötét pörköletek hullatnak — idővel kitömik a darálót, és a motor egyszerűen ráragad. A jel árulkodó: kiürítetted az adagolót, kiporszívóztad a garatot, a daráló mégis csak **zümmög, de nem forog**. Ha az út szabad, és a motor álló helyzetből mégsem indul, akkor a motor beragadt, és cserére szorul.

## A GIGA 6 kivétel

Mielőtt bármihez nyúlsz, egy fontos kivétel: a GIGA 6 esetében ugyanez az Error 12 kommunikációs vagy érzékelőhibára is utalhat, nem csak beszorulásra — ezt egy egyszerű újraindítással lehet elsőként kizárni. Ezért minden 12-es kódnál, típustól függetlenül, az első lépés a legolcsóbb: húzd ki a gépet, várj, indítsd újra.

## Elhárítás lépésről lépésre

1. Húzd ki a gépet öt percre, majd indítsd újra — GIGA 6 esetén önmagában ez is törölheti a kommunikációs hiba változatot.
1. Ürítsd ki teljesen a babadagolót, és nézd át az aljára került babokat: kavicsokat vagy összetapadt pörköletdarabokat keresve. Ha kavics akad a kezedbe, valószínűleg megtaláltad a hiba teljes okát.
1. Porszívózd ki szűk fúvókával az adagoló kifolyóját és a daráló garatját. Semmi fémet ne dugj a korongok közé: a karcolt darálókorong-készlet felesleges kiadás.
1. Ürítsd ki a zacctartót és a cseppgyűjtőt, tedd vissza mindkettőt, majd indítsd újra a gépet, hogy vissza tudja állítani magát a kiinduló helyzetbe.
1. Főzz egy kávét. Ha a daráló forog, megszűnt a blokkolás; ha az út már szabad, mégis csak zümmög, a motor beragadt, és cserélni kell.

## Mibe kerül

- **Darálómotor:** típus szerint 60–140 €.
- **Darálókorong-készlet:** 25–45 €, ha a beszorulás rongálta meg a korongokat.
- **Műhelyi javítás:** egy szuperautomata garancián kívüli gyártói szervizelése jellemzően 250–500 € a visszaszállítással együtt; egylakatrészes munkáknál a független kávégép-javítók általában olcsóbbak.

A korong- vagy motorexcsere egy GIGA-ban komoly szétszereléssel jár, ezért inkább műhelymunka, hacsak nem szervizelsz rendszeresen ilyen gépeket. A gyártói szolgáltatásokról a [Jura hivatalos honlapja](https://www.jura.com/hu/) tájékoztat. GIGA és Z gépeknél a javítás általában megéri; egy régebbi, kisebb modellnél mérlegeld az árajánlatot a gép értékével.

### Magyarországi praktikus tudnivalók

Itthon az új gépekre két év kötelező jótállás jár, ezért garanciális időben ne vedd fel a gép házát: a hálózat kihúzása, az adagoló kiürítése és a porszívózás nem minősül beavatkozásnak, a szétszerelés viszont elveszítheti a jótállást. Ha a tünetek motorberagadásra utalnak, fordulj a forgalmazóhoz vagy a gyártó magyarországi szervizpartnereihez árajánlatért. Mivel a hiba tisztán mechanikai, a hazai kemény csapvíz itt nem szerepel az okok között: a vízkő a fűtő- és szelephibák mögött áll, nem a 12-es mögött.

## A hiba után

Tegyél szokássá, hogy egy új zsák vagy egy új pörkölő első adagját átnézed, mielőtt az adagolóba töltöd — ekkor köt ki a legtöbb kavics. Az Error 12 megelőzése egyetlen mondatban: pillantsd át a babokat, mielőtt újratöltöd.

## Kapcsolódó kódok

Az Error 12 a Jura mechanikai hibacsaládjába tartozik, a főzőegység ciklushibáját jelző [Error 8](https://hu.codefixcoffee.com/jura/automatic-machines/error-8/) mellé, amely a barátságosabbik rokon: egy tisztítótáblás program jellemzően megoldja. Ugyanez a kavics-logika márkákon is átível: a De'Longhi gépek a beragadt darálót rejtett 1454-es kódként naplózzák, és a [beragadt daráló (1454) összefoglaló](https://hu.codefixcoffee.com/delonghi/magnifica-dinamica/grinder-stuck-code-1454/) ugyanezt a kiürítés-porszívózás eljárást írja le Magnifica és Dinamica tulajdonosoknak. Ennek az üzenetcsaládnak a többi tagja a [De'Longhi rovatban](https://hu.codefixcoffee.com/delonghi/) található; a Jura teljes számozott listája — a termoblokk-fűtő kódoktól a kerámia szelepig — a [Jura hibakód-összesítőben](https://hu.codefixcoffee.com/jura/) érhető el.
