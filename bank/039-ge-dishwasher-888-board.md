---
title: GE mosogatógép 888 és CFE: amikor a vezérlőelektronika a hibás
description: 888 vagy CFE a GE mosogatógépen? Mit takar a kijelző felülírása, hogyan zárható ki a nedves vezérlő, és milyen egyszerű a lapka cseréje.
---

A GE mosogatógépek kódjai többnyire valami nedvesre mutatnak: a C1 leeresztési időtúllépés (a leeresztő szivattyú nem vitte ki a vizet), a C6 fel nem melegedett víz, a H2O pedig azt jelenti, hogy egyáltalán nincs víz. Aztán ott a két kód, amely száraz, elektronikus hibára mutat. A [888](https://hu.codefixcoffee.com/ge/dishwasher/888/) azt jelenti, hogy a fő vezérlőelektronika megbukott a saját öntesztjén; a [CFE](https://hu.codefixcoffee.com/ge/dishwasher/cfe/) pedig azt, hogy az ajtóra szerelt kezelőpanel és a fő lapka megszakította egymással a kapcsolatot. Egyik sem eldugult szűrő valamiféle álcája. Ebben a bejegyzésben végigmegyünk azon, mit jelent valójában a kijelző átvétele, milyen vízellenőrzéseket érdemes megtenni a lapka megrendelése előtt, és milyen egy csere a valóságban.

## Mit jelent a 888-as kijelzés

Szegmenskijelzőn a 888 akkor látszik, ha minden számjegypozíció egyszerre világít. Nem hibaszám a C-kódok értelmében — a lapka azért gyújtja fel az összes szegmenst, mert megbukott a saját ellenőrzésén, és nem képes lefuttatni a normál programját. Ahol a [C1](https://hu.codefixcoffee.com/ge/dishwasher/c1/) azt jelenti, hogy "a szivattyú két percig futott, és a kád mégis tele maradt", addig a 888 azt, hogy maga az a számítógép hibás, amely ezt észrevette volna.

A szokásos kiváltó ok elektromos, nem mechanikus: egy vihar vagy generátorból érkező feszültségcsúcs megrongálja a lapka egyik memóriaregiszterét, és onnantól kezdve az önteszt minden gépindulásnál elbukik. Pontosan ezért éri meg a klasszikus tanács — a megszakítónál 60 másodpercre áramtalanítani, majd újraindítani — pontosan egy próbát, nem többet. A visszaállítás törli a futó hibát, de nem javítja meg a sérült memóriát. Ha a 888 a reset után visszatér, a kár már megtörtént, és a lapkát cserélni kell. Ritkábban nem feszültségcsúcs, hanem a lapkát beáztató szivárgás áll a háttérben — erre valók a lenti ellenőrzések.

## CFE: a másik elektronikai kód

A CFE kommunikációs hiba: az ajtóban elhelyezett kezelőpanel és a fő vezérlőelektronika vesztette el egymást. A jellemző gyanúsítottak: laza vagy átdörgölt kábelszakasz ott, ahol a vezeték az ajtópántnál hajlik, nedves csatlakozó, vagy a két lapka egyikének hibája. A diagnosztikai sorrend itt pénzben is mérhető, mert a két lapka másba kerül: először a megszakítós reset, utána (áramtalanítva) a kábelezés átnézése és a csatlakozók visszaültetése mindkét végén, a kopás keresésével ott, ahol az ajtó minden ciklusban mozog. Csak ép kábelezésnél érdemes lapkákra gyanakodni — a kezelőpanel cseréje a kettő közül jellemzően az olcsóbb. Modellfüggő eligazítást a [GE Appliances hivatalos weboldala](https://geappliances.com) is nyújt.

## Víz a lapkán: a tízperces ellenőrzés

Mielőtt bármilyen alkatrészt rendelnénk, tíz percet szánjunk a szivárgási út kizárására, mert a nedves gépbe épített új lapka is elhal:

1. Húzzuk ki a mosogatógépet annyira, hogy alá lehessen látni, és vizsgáljuk meg a padlót víz vagy kimosódási nyomok után.
1. Szereljük le az elülső lábazati burkolatot, és zseblámpával nézzünk be a gép aljába: a tálcában álló víz azt jelenti, hogy a szivárgás elérte a lapka környékét.
1. Nézzük végig a kézenfekvő forrásokat — a rossz mosogatószer habja, sérült ajtótömítés, repedezett tömlő, izzadó szivattyútömítés.
1. Ha bármi nedves, szárítsuk ki teljesen, és előbb a szivárgást javítsuk meg, utána reset és újrapróbálás. Az egyszer megfröcskölt és megszáradt lapka néha felépül; amely álló vízben ül, soha.

Ha minden csontszáraz, és a 888 vagy a CFE a 60 másodperces megszakítós reset után is visszajön, jöhet a lapkarendelés.

## A lapkacsere valósága

Az a jó hír, amit a "vezérlőelektronika" szó elrejt: GE mosogatógépeknél a lapka bedugható modul, nem forrasztott. Modellenként a lábazati panel mögött vagy az ajtó belsejében található, és a csere lényege ez:

1. Áramtalanítsunk a megszakítónál — ne csak a gép kapcsolójával —, mielőtt bármilyen panelt leverünk.
1. Nyissuk fel a lábazati panelt vagy az ajtófrontot, hogy szabaddá váljék a lapka.
1. Fényképezzük le a huzalozott csatlakozókat, mielőtt bármihez nyúlnánk.
1. Húzzuk le a csatlakozókat a régi lapkáról, szereljük fel az újat, és ugyanazon pozíciókban dugjuk vissza őket.

Forrasztás nincs, áthuzalozás nincs — a csatlakozók viszont sokan és felirat nélküliek, pontosan ezért fényképezzünk. A fő vezérlőelektronika €90–200, a kezelőpanel €60–120; a javítás tehát valós mérlegelés: hat-hét évnél fiatalabb gépen megéri, idősebb gépnél érdemes az új gép árával is összevetni. Aki nem maga csinálja, a technikusi kiszállással €120–250-rel többet fizet a diagnózisért, plusz az alkatrészért.

### Magyarországon: beszerzés és feszültség

GE mosogatógépet a magyar lakossági kereskedelemben gyakorlatilag nem kapni, így a vezérlőelektronikát is nemzetközi alkatrészboltokból kell rendelnünk — a szállítással és az esetleges vámdíjjal hetekkel érdemes számolni. Rendelés előtt mindig a gép adattábláján (az ajtó szélén) lévő pontos típusszám alapján keressünk lapkát, mert az amerikai variánsok egymástól is eltérnek. Ha pedig tengerentúlról származó, 120 V-os gépről van szó, azt soha ne kössük közvetlenül a 230 V-os magyar hálózatra — csak megfelelő transzformátoron keresztül.

A [GE mosogatógép-kódindex](https://hu.codefixcoffee.com/ge/dishwasher/) minden kódot lefed, de az elektronikai kódokra a döntési fa rövid: egy megszakítós reset, tíz perc szivárgás-ellenőrzés, majd vagy a kábelezés visszaültetése (CFE), vagy a lapkacsere. Ami soha: szűrőhiba, mosogatószer-hiba vagy egy harmadik reset.
