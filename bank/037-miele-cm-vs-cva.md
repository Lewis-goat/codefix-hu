---
title: Miele CM és CVA: azonos kódok, két eltérő gépcsalád
description: A Miele CM pulton álló és a CVA beépíthető kávégépei ugyanazokat az F-kódokat jelzik, de a hiba oka és a javítás költsége gépenként más.
---

A Miele két nagyon különböző formában gyártja kávégépeit. A **CM sorozat** — a CM 5510 és a CM 6150 — pulton álló gép: fali konnektorból működik, és kivehető víztartályból töltjük fel kézzel. A **CVA sorozat** — a CVA 6401 és a CVA 6805 — konyhabútorba építhető, és az ilyen gépeket gyakran a vízhálózatra kötik, nem kézzel töltik. Kívülről nem is lehetne nagyobb a köztük lévő különbség; belül viszont annyira rokonok, hogy a Miele mindkettőben ugyanazt a beépített öndiagnosztikát futtatja, és a hibákat mindkettő **F-kódokkal** jelzi.

Ez a közös hibatábla az oka annak, hogy egy F-kód ugyanazt jelenti egy pultos CM-ben és egy beépített CVA-ban. A sorozat azon változtat, melyik ok a legvalószínűbb, és a javítás mekkora részét végezhetjük el magunk.

## Egy hibatábla, két kézikönyv

A Miele a kódok jelentését minden sorozat üzemeltetési útmutatójában közli — a dokumentáció a [Miele hivatalos weboldalán](https://miele.com) is elérhető —, és a szöveg a pultos CM-füzetekben és a beépített CVA-füzetekben kicsit eltér. A kód mögötti öndiagnosztika ugyanaz; a leíró mondatok nem. Ha tehát a saját kézikönyvünk egy kifejezésére rákeresve a másik sorozat tanácsára esünk, olvassunk tovább: a közelítő találatot a szövegeltérés okozza, nem az, hogy más lenne a hiba.

A két kézikönyv az önjavítás határát is ugyanoda vonja. A Miele kifejezetten tiltja a külső burkolat felnyitását: a gépekben belső feszültségek és nyomás alatt álló vízrendszer van. Az F-táblán végig egységes a felosztás — a **vízellátási kódok azok, amelyeket a felhasználó maga megjavíthat**; a szelepes és a főzőegységes kódok jellemzően Miele-szervizt igényelnek. Ez a választóvonal CM- és CVA-tulajdonosként egyaránt érvényes.

## F10 és F17: a vízhiány, amely mindkét sorozatnál közös

Az F10 és az F17 egyetlen kézikönyvi bejegyzés alatt fut: a gép vizet próbált felvenni, és nem sikerült, vagy csak csepegésnyi folyt be. Ez a Miele-tábla legkezelhetőbb hibája, mert a kézikönyvi megoldás gyakran az egész megoldás. A sorozatok közti különbség csak az, honnan nem jött a víz.

Pultos CM-nél a gyanú szinte mindig a kivehető tartályra esik: üres, nincs rendesen a szelepére ültetve, vagy maga a szelep ragad be — mindhármat szerszám nélkül ellenőrizhetjük. Hálózatra kötött CVA-nál a gyanú felfelé vándorol, a vízvételi elzárószelepre és a csővezetéki szűrőre, mert itt nincs tartály, amely hibázhatna. A teendők sorrendje rövid:

1. Vegyük ki a víztartályt, töltsük meg friss, hideg csapvízzel, és tegyük vissza, amíg rögzül.
1. Nézzük meg a tartály szelepülését: a beragadt vagy szennyezett tömítést öblítsük át folyó víz alatt.
1. Hálózatra kötött gépnél ellenőrizzük, hogy a vízvételi elzárószelep teljesen nyitva van-e, és nincs-e eltömődve a szűrő.
1. Ha a hiba időnként visszatér, végezzük el a vízfelvételi rendszer mészetlenítését — a szelepben lerakódott mészkő miatt a hiba jön-megy.
1. Ha a kód bizonyítottan jó vízellátás mellett is fennáll, a felvételi szelepet vagy a szivattyút már a Miele szervizének kell megnéznie.

Költségben ez a hiba többnyire ingyenes; egy elromlott felvételi szelep €30–60 körül mozog. A [F10 és F17 oldala](https://hu.codefixcoffee.com/miele/cm-cva-machines/f10-f17/) a teljes eljárást lépésről lépésre végigveszi.

## F77: a belső hiba, amelytől mindkét sorozat tart

Az F77 a Miele gyűjtőkódja az induláskor észlelt belső hibára — a gyakorlatban leggyakrabban a szeleprendszer inicializálási problémája köré csoportosul. A kézikönyvi tanács őszintén jelzi az önjavítás határát:

1. Kapcsoljuk ki a gépet a be/ki-érzékelővel, majd húzzuk ki a fali konnektorból.
1. Hagyjuk kikapcsolva néhány percig; ha az F77 korábban rövid kikapcsolás után már visszajött, most adjunk neki akár egy órát.
1. Dugjuk vissza, kapcsoljuk be, és figyeljük: a hiba az inicializálásnál azonnal jelentkezik, vagy csak akkor, amikor italt kérünk?

A hálózati újraindítás után visszatérő F77 alkatrészhiba — szelep, szivattyú vagy vezérlőelektronika —, és a Miele szervizének dolga. Telefonálás előtt jegyezzük fel a típusszámot: a CM 5510/6150 és a CVA 6401/6805 belső felépítése eltér, tehát ugyanaz a kód nem ígéri ugyanazt a hibás alkatrészt. A szelep €50–120, a vezérlőelektronika ennél drágább. A [F77 oldala](https://hu.codefixcoffee.com/miele/cm-cva-machines/f77/) összegyűjti, mit érdemes rögzíteni, mielőtt hívjuk a szervizt.

## Pulton vagy szekrényben: a gyakorlati különbségek

- A CM kihúzható és arrébb tehető, ha kell a pult; a CVA rögzített beépítés, ezért minden beavatkozás előtt különítsük el az áramellátását.
- A CM vízútja egy kézben tartott tartálynál kezdődik; a CVA-é a szerelvényeknél — a "nincs víz" hibának ezért hosszabb az ellenőrizendő láncolata, és szivárgásnál a gép alatt ülő szekrény is veszélyben van.
- Garancián kívüli gyártói szervizteljesítmény teljesen automata gépnél jellemzően €250–500 között alakul a visszaszállítással együtt; a beépített egységet előbb ki kell emelni a burkolatból, mielőtt bárki árat mondhat — épp ezért érdemes a CVA vonalán a vízellátási hibákat korán elkapni.
- Egyetlen ismert alkatrész cseréjénél a független kávégép-javítók jellemzően olcsóbbak a gyártói útnál — de a Miele burkolatnyitásra vonatkozó figyelmeztetése arra érvényes, aki épp nyitja.

### Magyarországon: a kemény víz korábban hoz mészkövet

Magyarországon a csapvíz az ország nagy részében — Budapesten is — kifejezetten kemény, így a Miele-gépek vízutáján a mészkőlerakódás és a mészetlenítés szükségessége jóval korábban jelentkezik, mint a gyári átlag. Az időnként visszatérő, F10/F17-jellegű vízfelvételi hibáknál ezért nálunk különösen fontos a rendszeres mészetlenítés, illetve lágy, szűrt víz használata a tartályos CM-eknél. Hálózatra kötött CVA telepítésekor érdemes a szerelővel vízpuhítót vagy szűrőbetétet is beépíttetni.

A [Miele-szekció](https://hu.codefixcoffee.com/miele/) többi része mindkét sorozat üzemeltetési útmutatóját követi, és jelzi a szövegeltéréseket, ahol felbukkannak.
