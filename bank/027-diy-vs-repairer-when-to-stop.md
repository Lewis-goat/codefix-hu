---
title: Szerviz vagy saját kezű javítás? A nehézség őszinte mérlegelése
description: Hogyan döntsd el egy hibakódról, hogy barkácsolható-e a javítás. Veszély vagy nehézség, stopjelzések, biztonsági csavarok és költségszámítás.
---

A kijelzőn hibakód, a gépkönyv tanácsa nem segített, és a kérdés hirtelen személyessé válik — megjavítod magad, vagy fizetsz valakinek? A döntés nagyjából nem a kézügyességedről szól, hanem a hibáról. Két, egymástól független ítéletre bontható: mennyire veszélyes ez a hiba, és mennyire nehéz a javítás?

## A veszélyesség nem egyenlő a nehézséggel

A **veszélyesség** azt mondja meg, mennyire sürgős a gép használatát abbahagyni — a tűz- és vízkár, valamint annak kockázata, hogy a hiba magával ránt más alkatrészeket is. A **nehézség** azt, hogy a javítás mit kíván tőled: szerszámokat, hozzáférést, és hogy mi romolhat el útközben. Ez két független skála, és összetévesztésük pánikhoz éppúgy vezet, mint a felhőtlen nyugalomhoz.

- **Súlyos, de kezelhető.** A [GE mosogatógép E1 kódja](https://hu.codefixcoffee.com/ge/dishwasher/e1-leak/) azt jelenti, hogy a gép aljában lévő vízbiztonsági úszókapcsoló lépett működésbe — magas veszélyesség, és a gép nem fut tovább, amíg az alap száraz nem lesz, és a szivárgást meg nem találod. Az első lépések akkor is egyszerűek: zárd el a vizet, válaszd le az áramot, vedd le a lábazati panelt, és szárítsd ki az alapot.
- **Drámai, de mérsékelt.** A [Jura 8-as hibája](https://hu.codefixcoffee.com/jura/automatic-machines/error-8/) holtra állítja a gépet, mert a főzőegység nem fejezte be a ciklusát. Összeomlásnak tűnik, mégis a legtöbb esetben tisztítási feladat — a 8-as hibák többsége egy doboz tablettába kerül.
- **Súlyos és igazán nehéz.** A [Jura 7-es hibája](https://hu.codefixcoffee.com/jura/automatic-machines/error-7/) — a szelep nem érte el a vezérlőelektronika által kívánt pozíciót — azon kevés Jura-kód egyike, amelyre nincs megbízható felhasználói megoldás.
- **Első pillantástól szóba sem jöhet.** A [Miele F77](https://hu.codefixcoffee.com/miele/cm-cva-machines/f77/) belső szelephiba, amelynél a hivatalos megoldás az áramtalanításnál és visszakapcsolásnál megáll, a ház felnyitása pedig kifejezetten tiltott — belső feszültségek és nyomás alatt álló vízkör miatt.

A munkaszabály: a veszélyesség dönti el, **megállsz-e**; a nehézség dönti el, **ki végzi a munkát**.

## Mikor stopjelzés a kód

Van néhány helyzet, amely a barkácsolási fázist még a szerszámok előtt befejezi, legyél bármekkora önbizalommal:

- **Víz az elektronika helyén.** Egy mosogatógépes úszókapcsoló-kód, mint az E1, azt jelenti, hogy a gép nem fut le újra, amíg az alap száraz nem lesz, és a szivárgást nyomon nem követted — nem „még egy program, hátha".
- **Fűtő, amely nem kapcsol ki.** Az ismétlődő túlhőmérséklet-kód komoly változata, amikor a teljesítményelektronika nem képes leválasztani a fűtőelemet. Tűzkockázatként kezeld: húzd ki a gépet, és ne hagyd felügyelet nélkül áram alatt.
- **A gyártó saját határa.** Ha egy kód dokumentált megoldása az áramtalanítás, majd utána a „forduljon szervizhez", a kézikönyv pedig kimondja, hogy a házat nem szabad lebontani — a gyártó éppen megmondta, hol húzódik a határ és a te biztonsági tartalékod.
- **Visszatérés a szabályos visszaállítás után is.** Áramtalanítsd a kávégépet öt percre, vagy kapcsold ki a mosogatógépet a megszakítón hatvan másodpercre. Ha a kód a ciklus ugyanazon pontján tér vissza, egy alkatrész bukik meg a saját ellenőrzésén — nem kósza jelenség.

## Hálózati feszültség és biztonsági csavarok

A hozzáférés a kávégépeknél a nehézség legőszintébb fejezetéhez tartozik. A Jura házakat tojásfejű Torx-Plus biztonsági csavarok tartják, a belsejükben a termoblokk kapocsai hálózati feszültséget vezetnek. A 7-es hiba szelepcsérléséhez való alkatrészeket bárki megveheti, de a beépítés biztonsági csavarokat, élő oldal iránti tudatosságot és a mechanizmus utána történő újrakalibrálását jelenti — az őszinte ítélet ennél a kódnál műhelymunka, hacsak nem szerelsz már rendszeresen ilyen gépeket. Ha nincs meg a szerszám, kezeld a házat zártként; szerszámokhoz és szétszerelési példákhoz jó kiindulópont az [iFixit](https://www.ifixit.com) adatbázisa.

Ugyanez a fegyelem érvényes a lakás többi pontján is. A gépet a falaljzatról vagy a megszakítóról válaszd le, ne a saját kapcsolójával. És soha ne kerüld meg egy biztonsági elemet: a hőbiztosíték azért van, hogy tönkremenjen — áthidalásával nem tanulsz semmi olyat, amit tudni akartál.

## A költségek számítása

Mielőtt utat választasz, árazd be mindhármat:

1. **Az ingyenes kísérlet.** Visszaállítás, tisztítási program, alkatrész újraültetése, mészetlenítés. Nem kerül semmibe, és a mindennapi kódok nagy részét eltünteti.
2. **A saját kezű javítás.** Ide jön az alkatrész, a szerszám és a félrediagnosztizálás kockázata. Tisztítószer-tabletta 15–25 €, egy Jura főzőegység 80–150 €, egy kerámiaszelep-egység modelltől függően 60–150 €.
3. **A szerelő.** A garancián kívüli gyártói szerviz egy szuperautomatánál jellemzően 250–500 €-ba kerül a visszaszállítással együtt, és a független eszpresszó-szerelők egy alkatrészes munkára általában olcsóbbak. Egy háznál járó műszaki szerelő 120–250 €-t kér a diagnosztikáért, plusz az alkatrész.

Aztán vesd egybe a teljes összeget a gép értékével. A csúcs [Jura](https://hu.codefixcoffee.com/jura/) Z és GIGA modelleknél még a szervizi sáv teteje is általában kifizetődő; egy tízéves belépő E vagy ENA gépnél az árajánlatot vesd össze egy felújított egységgel. Azt is nézd meg, hol dominál a munkadíj — a 7-es hibánál a szerelési munkadíj jellemzően meghaladja az alkatrész árát.

### Jótállás és szakszerviz Magyarországon

Új készülékekre Magyarországon jogszabályi kötelező jótállás jár, amely kávégépeknél jellemzően egy év. A ház felnyitásával ez a jótállás jó eséllyel elúszik, ezért garancián belül vidd a gépet hivatalos márkaszervizbe, ne szereld magad. A jótállás lejárta után a független műszaki szervizek jóval olcsóbb alternatívát kínálnak — a hálózati feszültséggel járó beavatkozásokat viszont érdemes szakemberre bízni, ahogy a gyártók, például a [Miele hivatalos webhelye](https://www.miele.com) is javasolja.

A kód azzal, hogy megnevezte az érintett áramkört, már elvégezte a dolgát. Először a veszélyességet ítéld meg, és állj meg, ha azt diktálja. Utána a nehézséget, és hagyd, hogy a szerszámosládád és a javítás közti távolság döntsön arról, ki végezze el a munkát.
