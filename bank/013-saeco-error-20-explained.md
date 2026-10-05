---
title: "Saeco 20-as hiba: főzőegység, ajtókapcsolók, és miért fontos, hogy minden a helyén kattanjon"
description: "A Saeco 20-as hibakód a főzőegységre vagy az ajtókapcsolókra hívja fel a figyelmet: itt a dokumentált reset, a főzőegység tisztítása és a motor szerepe."
---

A Philips és a Saeco szuperautomata kávégépeken a 20-as hibakód elsőre komolyabbnak hangzik, mint amennyire a legtöbb esetben valójában az. A LatteGo 2200/3200/4300/5400, az Xelsis, az Incanto és a régebbi Saeco modellek közösen azt az 01-től 22-ig terjedő tartományt használják, amelyből a Xelsis generáció kézikönyvei a 20-ast két irányba terelik: a főzőegység felé, illetve a cseppgyűjtő tálcát, a kávézacc-tartályt és a szervizajtót figyelő kapcsolósor felé. Részletes összefoglalónkat az [Error 20 referenciaoldalon](https://hu.codefixcoffee.com/philips-saeco/espresso-machines/error-20/) találja; e bejegyzés azt fejti ki, mitől döntő, hogy minden alkatrész pontosan a helyén ül — és mikor van mélyebb gond a háttérben.

## Mit jelz valójában a gép

A Philips nem tesz közzé kódonkénti táblázatot a szervizkódjairól, ezért a szervizrészlegen kívül senki nem ígérheti meg, hogy minden típuson ugyanazt az alkatrészt nevezi meg a 20-as hiba. A Xelsis-korszak kézikönyvei viszont egyértelműen mutatnak az irányt: az e tartományba eső numerikus kódok arra utalnak, hogy a vezérlőelektronika nem érzékeli a főzőegységet a helyén, vagy hogy egy szervizelem — a cseppgyűjtő tálca, a kávézacc-tartály, a szervizajtó — nincs teljesen behelyezve.

Minden főzőciklus előtt és közben a gép egy biztonsági kapcsolósort és a főzőegység pozícióérzékelőjét ellenőrzi. Ha bármelyik azt jelenti, hogy valami nincs rendben, a ciklus leáll, és a kijelzőn megjelenik a 20-as hiba:

- a főzőegységnek jelen kell lennie, és a nyugvó helyzetben kell lennie
- a cseppgyűjtő tálcának teljesen be kell csúsznia a helyére
- a kávézacc-tartálynak a tálcára helyezve, kattanásig kell rögzülnie
- a szervizajtónak teljesen zártnak kell lennie

Ez nem kényeskedés. A szuperautomata a főzőegységet valódi mechanikai ciklusban mozgatja, és nyitott ajtóval vagy félig bekötött egységgel bele sem kezd. A gyakorlatban a 20-as hibák jelentős része egy néhány milliméterrel rövidebbre csúsztatott tálcára vagy nedves kávézacca vezethető vissza, amely érintkezők között hidat képez.

## A dokumentált reset: öt perc, alkatrész nélkül

1. Kapcsolja ki a gépet, és húzza ki a hálózati dugaszát.
2. Vegye ki a cseppgyűjtő tálcát és a kávézacc-tartályt, majd helyezze vissza mindkettőt határozott mozdulattal, kattanásig.
3. Zárja be teljesen a szervizajtót.
4. Kapcsolja be újra a gépet.

Ez a visszaállítási eljárás szerepel a kézikönyvben ehhez a hibacsaládhoz, és az újraüléses újraindítás tényleg a legtöbb esetet megoldja. Ha a kód ezután eltűnik, készen van — de azért olvassa el a következő részt is, mert az ismétlődő 20-as hiba mindig valamilyen háttérben álló okra hívja fel a figyelmet.

### Ha visszatér: tisztítsa meg a főzőegységet

Olyan gépeken, amelyeken a főzőegység kivehető (a LatteGo és Incanto modellek többsége), a következő gyanúsított maga az egység:

1. Kapcsolja ki a gépet, nyissa ki a szervizajtót, és vegye ki a főzőegységet.
2. Öblítse át alaposan langyos vízzel — szappan nélkül —, majd hagyja levegőn megszáradni.
3. Kenjen kevés élelmiszer-biztos szilikonzsírt a vezetősínekre és a dugattyú tömítésére.
4. Csúsztassa vissza a sínek mentén kattanásig, zárja be az ajtót, és kapcsolja be a gépet.

Ezek után indítson egy öblítőciklust. Ha a kód eltűnik, futtassa le a gép tisztítóprogramját is: a kávéolajoktól ragacssá vált főzőegység az ismétlődő 20-as hibák leggyakoribb kiváltó oka, és pontosan ez az, amit a tisztítóciklus kezeli. Egy óvatossági megjegyzés: azokon a Xelsis modelleken, amelyekben a főzőegység beépített és nem kivehető, ne erőltesse a szervizajtót, hogy hozzáférjen — a javításnak az a változata műhelymunka.

A szomszédos kódok is hasonló történetet mesélnek: a 03-as a „főzőegység túl szennyezett" kód, a 04-es pedig a „főzőegység nincs helyesen behelyezve" — a teljes családot a [Philips / Saeco gyűjtőoldal](https://hu.codefixcoffee.com/philips-saeco/) fogja össze.

## Mikor a motor vagy a pozícióérzékelő a hibás

Ha a 20-as hiba akkor is fennáll, hogy a tálca, a tartály és az ajtó bizonyítottan a helyén van, az egység pedig tiszta és zsírozott, megváltozik a kép: vagy a főzőegység motorja nem képes végigvinni a ciklust, vagy a pozícióérzékelő nem olvassa vissza azt. Mindkettő belső beavatkozás — a [Philips hivatalos támogatási csatornája](https://www.philips.com/support) ezeket szervizbe irányítja —, és egyikhez sincs értelme felhasználói szintű javítási kísérletbe belemenni. Ha kíváncsi, mi lapul a gép belsejében, az [iFixit lépésről lépésre dokumentált szétszerelési útmutatói](https://www.ifixit.com) jó kiindulópontok, de a főzőegység-meghajtó cseréje műhelyi feladat.

Ne keverje össze ezt a másmilyen, szintén komoly Saeco hibacsaláddal. A 02, 10, 15 és 22 a gép belsejében lévő elektronikai, szivattyú- és szelephibák kódja, amelyeket a Philips eleve szervizbe utal. Hasznos támpont az időzítés: a bekapcsoláskor jelentkező kódok többnyire a főzőegység-meghajtóra vagy egy szelepre utalnak, a főzés közben jelentkezők pedig a szivattyúra vagy a nyomási oldalra. A részleteket az [Error 02, 10, 15 és 22 oldal](https://hu.codefixcoffee.com/philips-saeco/espresso-machines/error-02-10-15-or-22/) tartalmazza.

## Milyen költséggel érdemes számolni

- Szilikonzsír: kb. 10 € — és a legtöbb 20-as hibához valójában ennyi az egyetlen szükséges „alkatrész".
- Csere főzőegység, ha a meglévő sérült: nagyjából 80–140 €.
- Garancián kívüli gyári szerviz szuperautomatáknál: jellemzően 250–500 €, a visszaszállítást is beleértve; önálló kávégép-javítóknál egyetlen alkatrész cseréje általában olcsóbb.

Xelsis vagy LatteGo osztályú gépnél a javítás megéri — és jó eséllyel soha nem jut el a harmadik pontig. Kezdje az [Error 20 oldalon](https://hu.codefixcoffee.com/philips-saeco/espresso-machines/error-20/), végezze el a resetet a megadott sorrendben, és csak akkor fogjon a telefonhoz, ha már minden tiszta, zsírozott és a helyén kattan.

### Magyarországi gyakorlati megjegyzés

Magyarországon a csapvíz az ország nagy részén — Budapesten is — kemény, magas ásványianyag-tartalmú, ami a kávéolajak mellett felgyorsítja a főzőegység ragacssá válását, ezért érdemes az egységet hetente kiemelni és átöblíteni. A vásárlási számlát őrizze meg: a magyar kellékszavatosság a vásárlástól számított két évig áll fenn, és garanciális szerviz esetén a vásárlás időpontját kell igazolni.
