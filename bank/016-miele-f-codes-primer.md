---
title: "Miele F-kódok: alapozó CM és CVA géptulajdonosoknak"
description: "Hogyan működik a Miele CM és CVA kávégépek F-kódos öndiagnosztikája, mely vízellátási hibákat javíthatja meg maga, és miért kell szerviz az F77-hez."
---

## Hogyan működik a Miele öndiagnosztikája

A Miele asztali CM gépei és beépíthető CVA kávégépei folyamatosan felügyelik a saját töltési ciklusaikat, a szelepeket és a főzési alkatrészeket, és ha egy önteszt elbukik, a gép F-kóddal jelzi. A rendszer logikája szokatlanul átlátható, ha egyszer megértette: a kódok olyan hibákra oszlanak, amelyek fizikailag elérhető helyeken vannak — víztartály, ellátó vezeték, szűrő —, és amelyek a gép belsejében rejlenek, ahol a kézikönyv válasza egy áramkör-megszakítás, majd a Miele szerviz.

Ez a határ érvényes szabály, nem javaslat. A Miele egyértelműen kimondja, hogy a külső burkolat nem nyitható fel: a gépek belső feszültségeket és nyomás alatt álló rendszert tartalmaznak. Egy Miele-tulajdonos igazi tudománya ezért nem az alkatrészdiagnosztika, hanem a szűrés — annak felismerése, mely kódok az öné, és melyek a szervizé. A modellek belső felépítésben eltérnek (egy CM 5510 vagy 6150 asztali egység más gép, mint egy CVA 6401 vagy 6805 beépített), de az F-kódos szemlélet közös, ezért egy alapozó a teljes választékon hasznos. A teljes listához induljon a [Miele rovatunktól](https://hu.codefixcoffee.com/miele/).

## A barátságos vég: az F10 és F17 vízellátási kódok

Az F10 és az F17 közös kézikönyv-bejegyzés alatt fut, és a megfogalmazást érdemes szó szerint ismerni: a gép egyáltalán nem, vagy csak nagyon kevés vizet tud beszívni. Vagyis megpróbált tölteni, és vagy teljesen elbukott, vagy csak csöpögött. Ez a Miele-tábla legkezelhetőbb hibacsaládja, mert a kézikönyvi javítás csaknem minden alkalommal önmagában a teljes megoldás.

Hová nézzen először, az géptípustól függ:

- **Asztali CM gépek:** az ok csaknem mindig a kivehető tartály — üres, rosszul ülő, vagy beragadt szelepű.
- **Vezetékes CVA gépek:** a gyanú a gép előtti elzárószelepre és az előtét-szűrőre tolódik át.

Mindkét típusnál rövid a teendők listája:

1. Vegye ki a víztartályt, töltse fel friss, hideg csapvízzel (ne desztillálttal), és helyezze vissza, amíg rögzül — ez szinte szó szerint a kézikönyv megoldása.
2. Ellenőrizze a tartály szelepülését: a beragadt vagy szennyezett tömítést öblítse át folyó víz alatt.
3. Vezetékes gépnél győződjön meg róla, hogy az elzárószelep teljesen nyitva van-e, és az előtét-szűrő nincs-e eltömődve.
4. Ha a hiba visszatér, mészetlenítse a vízbeömlőt — a szelepben lerakódott mész az, ami időnkéntessé teszi ezt a hibát állandó helyett.
5. A gép, amely igazolt vízellátás mellett is jelzi a kódot, beömlő szelep- vagy szivattyúvizsgálatot igényel a Miele szerviztől.

Itt a költség minimális: jellemzően 0 €, és csak akkor merül fel alkatrészár, ha a beömlő szelep valóban tönkrement — nagyjából 30–60 €. Az [F10 és F17 részletes oldalunk](https://hu.codefixcoffee.com/miele/cm-cva-machines/f10-f17/) a tartály- és vízvezeték-ellenőrzéseket teljes részletességgel mutatja be.

## A szervizhatár: az F77 és a belső hibák

A tábla másik oldalán ül az F77, a Miele gyűjtő kódja a bekapcsoláskor észlelt belső hibára — a gyakorlatban leggyakrabban a szeleprendszer inicializációs hibájára. A kézikönyv javaslása őszintén jelzi az önjavítás határait:

1. Kapcsolja ki a gépet a be-/kikapcsoló érintőszenzorral, majd húzza ki a hálózati dugaszt a fali aljzatból.
2. Hagyja kikapcsolva néhány percig; ha az F77 korábban egy rövid kikapcsolás után már visszatért, adjon neki akár egy órát.
3. Dugja vissza és kapcsolja be, közben figyelje, hogy a hiba az inicializálásnál azonnal jelentkezik-e, vagy csak ital kérésekor bukik fel.

Az F77, amely az áramkör-megszakítási kísérlet után is visszatér, alkatrészhiba — szelep, szivattyú vagy a vezérlőelektronika —, és határozottan a Miele szerviz dolga. Hívás előtt jegyezze fel a típusszámot, mert a CM és CVA gépek belsőleg különböznek, és a szervizrájt ez elsőként fogja elkérni. Az [F77 referenciaoldalunk](https://hu.codefixcoffee.com/miele/cm-cva-machines/f77/) összefoglalja, mit érdemes ellenőrizni és mire számítani; a gyártó hivatalos támogatása a [Miele támogatási oldalán](https://www.miele.com) érhető el.

## Egy megjegyezhető szabály a kódok szűréséhez

Az F-család e két bejegyzésen túl is folytatódik, beleértve a szelep- és főzőegység-hibákat, amelyek ugyanabba a szervizhatárba esnek, mint az F77. A tábla memorizálása helyett alkalmazzon egyetlen szabályt: ha a javítás olyan vízhez nyúl, amelyet lát — tartály, elzárószelep, szűrő —, az az Ön dolga, és a kézikönyv lépései megoldják. Ha a javítás a gép kinyitását jelentené, vagy egy kód a teljes áramkör-megszakítás után is visszatér, az a Miele-é.

A javításgazdaság is ezt a felosztást támasztja alá. Egy szelepcsere ezeken a gépeken kb. 50–120 €, a vezérlőelektronika ennél többbe kerül, de a CM és CVA rendszerek ára miatt a javítás jellemzően jobban megéri, mint a csere — és az áramkör-megszakítási kísérlet ingyenes, tehát a hívás előtt mindig megér egy próbát. A kódokhoz tartsa könyvjelzők között az [F10 és F17 oldalt](https://hu.codefixcoffee.com/miele/cm-cva-machines/f10-f17/) és az [F77 oldalt](https://hu.codefixcoffee.com/miele/cm-cva-machines/f77/): együtt lefedik azokat a hibákat, amelyekkel géptulajdonosként ténylegesen találkozhat.

### Magyarországi gyakorlati megjegyzés

A magyar csapvíz keménysége miatt a vezetékes CVA gépek előtét-szűrőjét érdemes a gyári ütemzésnél sűrűbben ellenőrizni, a tartályos CM gépekbe pedig Miele eredeti vízszűrőt vagy szűrt vizet érdemes használni — ez lassítja a mészlerakódást, és ezzel az F10/F17 jellegű, időnkéntessé váló hibákat. Mielőtt szervizt hívna, jegyezze fel a gép adattábláján lévő típusszámot: a Miele magyarországi ügyfélszolgálata ezt kéri elsőként.
