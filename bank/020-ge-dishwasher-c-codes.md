---
title: "GE mosogatógép C kódok: leeresztési, vízkészülési és fűtési hibák"
description: "A GE mosogatógép C1–C8 kódjai a leeresztést, a vízbeeresztést és a fűtést fedik le; a 888 és CFE a vezérlőelektronikát jelzi."
---

A GE mosogatógépek a hibáikat C-kódokként jelentik a kijelzőn: C1-től C8-ig, emellett H2O a vízkészülési problémákra, illetve 888 vagy CFE, ha maguk a panelek panaszkodnak. A legtöbb gyártóval ellentétben a GE nem ad ki hivatalos kódlistát, így a tulajdonosokra marad, hogy két karaktert párosítsanak a tünethez — némi támpontot a [GE Appliances hivatalos honlapjának](https://geappliances.com) terméktámogatása adhat. A [GE mosogatógép rovatunk](https://hu.codefixcoffee.com/ge/dishwasher/) minden kódot tárgyal; ez a bejegyzés végigmegy a családokon abban a sorrendben, ahogyan találkozhat velük, és egy szervizmenü-trükkel zár, amellyel kiolvasható az utoljára tárolt hiba.

## A leeresztés családja: C1–C3

Három kód, egy rendszer. A C1 jelentése: a leeresztő szivattyú két percnél tovább futott anélkül, hogy a medencét kiürítette volna (néhány régebbi modellen ragadt gombot jelez); a C2 azt, hogy a szivattyú egyáltalán nem indult el, vagy a vonal teljesen el volt dugulva; a C3 az általános „nem ereszti le rendesen” bejegyzés. A gyanúsítottak listája sosem változik: eltömődött szűrő és szivattyúmedence, gyűrődött leeresztő tömlő, nemrég beszerelt hulladékdaráló, amelyből a csatlakozócsonk fedőbélyegét nem ütötték ki, vagy tönkrement leeresztő szivattyú. Kezdje a szabad munkával a [C1 oldalon](https://hu.codefixcoffee.com/ge/dishwasher/c1/): húzza ki az alsó kosarat, tisztítsa meg a szűrőt és a medencét, és nézze meg a tömlőt a mosogató alatt. A leeresztő szivattyú €40–€80, ha kiderül, hogy zúg vagy néma.

## Vízbeeresztési hibák: C4, C5 és H2O

- **C4** — túlcsordulás, vagy a gép áramkimaradás után kétszer töltötte fel magát. A beömlő szelep nem zár rendesen, vagy az úszókapcsolót törmelék ragasztotta be. A [C4 oldalon](https://hu.codefixcoffee.com/ge/dishwasher/c4/) az úszóellenőrzés található; ha a medence kikapcsolt gépnél is töltődik, a beömlő szelep átereszt, és cserélni kell (€25–€50).
- **C5** — alacsony vízszint: a megadott idő alatt nem jött össze elég víz. Részlegesen zárt elzáró csap, eltömődött előszűrő vagy gyenge beömlő szelep.
- **H2O** — egyáltalán nincs víz. Mielőtt bármihez nyúl, nézze meg, hogy a mosogató alatti elzáró nyitva van-e, és nem gyűrődött-e a tömlő.

## Fűtési hibák: C6–C8

A C6 azt jelzi, hogy a víz a meghosszabbított fűtési idő letelte után sem érte el a kb. 49 °C-ot (120 °F). Indítás előtt engesse el a konyhai csapot, amíg meleg nem lesz — ha a víz hidegen érkezik, előfordulhat, hogy a fűtőelem egyszerűen nem tudja behozni. Ha az edények hidegen és vizesen jönnek ki, mérjen folytonosságot a fűtőelemen; az elem €30–€60, a hőhatároló termosztát €10–€20. A C7 a vízhőmérséklet-érzékelő (NTC hőérzékelő) körének hibája — kilazult dugasz vagy olcsó szonda, bár egyes modelleken ugyanez a kód a zavarosságérzékelőt fedi. A C8 jellemzően mechanikus, nem hőtani ok: az adagolókanalat nem tudta kinyitni, mert egy rosszul betöltött edény útban volt, vagy a kiszáradt mosogatószer beleragadt a zárba.

## 888 és CFE: a panelek kódjai

Amikor a hiba elektronikai és nem hidraulikai, a GE kerek szavú. A [888](https://hu.codefixcoffee.com/ge/dishwasher/888/) azt jelenti, hogy a fő vezérlőelektronika megbukott a saját öntesztjén — gyakran egy viharból jövő feszültségcsúcs írja felül egy memóriaregiszterét, néha pedig szivárgás nedvesíti be a panelt. A [CFE](https://hu.codefixcoffee.com/ge/dishwasher/cfe/) azt, hogy az ajtón ülő kezelőpanel és a főpanel megszűnt beszélni egymással, jellemzően az ajtópánt környékén kidörzsölt kábelszett vagy nedves csatlakozó miatt. Mindkettő automatamegszakítós újraindítással kezdődik, és panellel végződik, ha a kód visszatér: €90–€200 a fő vezérlőelektronika, €60–€120 a kezelőpanel.

## A szervizmenü trükkje: az utolsó hiba kiolvasása

Egy mosogatógép, amely hetek óta leállásokkal dolgozik, gyakran pontosan akkor nem mutat semmit, amikor az ember elé áll. A panel emlékszik — a legtöbb GE mosogatógépen meg is lehet kérdezni:

1. Nyissa ki teljesen az ajtót.
1. Tartsa nyomva a Start gombot öt másodpercig a szervizmenübe lépéshez.
1. Azokon a modelleken, ahol a kijelző az ajtó díszléce mögé rejtve van, nyomja egyszerre a Select Cycle és a Start gombot öt másodpercig.
1. Olvassa le a kijelzőről az utolsó tárolt hibát, majd csukja be az ajtót.
1. A panel alaphelyzetbe tételéhez kapcsolja ki az automata megszakítón 60 másodpercre.

Jegyezze fel a kódot, törölje, és indítson egy programot: egy három hete tárolt C3 plusz egy mai friss C3 valódi leeresztési hiba, nem véletlen egyezés.

### Magyarországi vásárlóknak: ellenőrizze a típustáblát

A GE mosogatógépek nálunk jellemzően amerikai importból kerülnek a konyhákba, és a típusok többsége 120 V, 60 Hz hálózatra készült. A magyar 230 V, 50 Hz hálózaton az adattábla szerinti feszültség nélkül a gép nem üzemel biztonságosan: a 120 V-os példányhoz megfelelő teljesítményű transzformátor kell, és az 50 Hz-en forgó motorok, szivattyúk viselkedése is eltérhet. Mielőtt bármit javítana vagy alkatrészt vásárolna hozzá, olvassa le az ajtó szélén lévő típustáblát, és győződjön meg róla, hogy a gép paraméterei összeegyeztethetők-e az itthoni hálózattal.

## Mibe kerülnek a javítások

Hozzávetőleg minden C-kód javítása egy szivattyú, egy szelep, egy érzékelő vagy egy adagoló — €10 és €80 közötti alkatrészek —, plusz a saját munka, ha vállalja az áramtalanítást és egy panel levételét. Kivétel a vezérlőelektronika €90–€200 közötti árával. Egy házhoz hívott gépszerelő diagnózisa €120–€250 plusz az alkatrész — ez a paneles kódoknál megéri, egy eltömődött szűrőnél ritkán szükséges.
