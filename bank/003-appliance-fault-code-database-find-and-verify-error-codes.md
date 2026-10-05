---
title: Hogyan találja meg és ellenőrizze egy gép hibakódjának jelentését
description: Rendszerezett módszer: hol rejtik a gyártók a kódlistákat, hogyan egyeztethető a fórum a szervizdokumentummal, és miért megtévesztő az ugyanolyan kód.
---

A kijelzőn látott kód csak a válasz fele: jelzi, hogy a gép hibát észlelt, de ritkán mondja meg, melyik alkatrészt kell megvenni. A kód a vezérlőelektronika programozója által írt tünetleírás — és ami a hibát észleli, a jelentését el is vétheti. Mielőtt bármit rendelne, szerezze be a jelentést a saját márkájára, géptípusára és modelljére, méghozzá több forrásból.

## A gyártói listák léteznek — csak el vannak ásva

Az első meglepetés az, hogy milyen gyakran nincs hivatalos lista egyáltalán, vagy ott rejtőzik, ahol a tulajdonosok sosem keresnek:

- Vannak márkák, amelyek semmit sem közölnek. A GE mosogatógépek C-kódokat, H2O-t és 888-at mutatnak, hivatalos hibakód-oldaluk még sincs; az űrt javítóoldalak töltik ki. A GE mosogatógép [888 kódja](https://hu.codefixcoffee.com/ge/dishwasher/888) vezérlőelektronika-hiba — ezt a GE-től nem fogja megtudni.
- Vannak, akik kettéosztják az információt. A De'Longhi gépek többnyire szavakat jeleznek, például General Alarmot, az újabb modellek viszont olyan számú kódokat is naplóznak, mint az 1101 vagy az 1512, amelyeket normál esetben csak a technikusok látják; a két réteg együtt szerepel a [De'Longhi General Alarm és számkódok oldalán](https://hu.codefixcoffee.com/delonghi/magnifica-dinamica/general-alarm-code-1101-1512).
- Vannak, akik csak a barátságos részt publikálják. A Philips a kávégépeihez kevés, felhasználó által javítható kódot listáz, a többit a támogatáshoz irányítja — holott a "szerviz" kódoknak is azonosítható okuk van; a gyártő saját oldalát itt érdemes kezdeni: [Philips](https://www.philips.com).
- Ahol a kézikönyvben van táblázat, az rendszerint a kötet végén, a hibaelhárítási fejezetben bújik meg, soronként egy kód, alkatrésznév és teendő nélkül.

Az információ tehát a legtöbbször létezik — csak a gyors kezdő útmutatón túl kell nézni.

## Hogyan ellenőrizzen úgy, mint egy technikus

### Írja le pontosan, mit mutat a kijelző

Rögzítse a pontos karakterláncot, a gép típusát, a jelzőtáblán szereplő teljes típusszámot és azt, mikor jelenik meg a kód. Egyetlen rosszul olvasott számjegy a rossz alrendszerhez visz. A Samsung tűzhelyeken és sütőkön az SE az érintőpanel membránjának beragadt gombját jelenti — részletesen a [Samsung SE magyarázatában](https://hu.codefixcoffee.com/samsung/range-wall-oven/se) —, más géptípusokon a hasonló karakterek egészen máshová mutatnak.

Jegyezze fel azt is, hogy indításkor vagy ciklus közben bukkan-e fel a kód: az indításkorit a bekapcsolási önteszt fogja el, a ciklus közbenit többnyire az éppen aktív komponens okozza — szivattyú, fűtőelem vagy szelep. Azt is figyelje, mitől tűnik el: a Samsung sütők például addig tartják a kódot, amíg az okot meg nem szüntetik, vagy amíg a megszakítón le nem vágták az áramot három percre; a teljes lista a [Samsung sütő hibakódok oldalon](https://hu.codefixcoffee.com/samsung-oven-error-codes/) van indexelve.

### Először a gyártó jelentése

Nézze meg a hibaelhárítási fejezetet, a márka alkatrész- és szervizportálját — például a [GE hivatalos oldalát](https://www.geappliances.com) —, majd a modellhez kiadott szervizközleményeket, még mielőtt fórumra menne. A hivatalos jelentés az alapvonal; minden más csak kommentár.

### Fórum a szervizdokumentáció mellé

A fórumtémákban derül ki, mi romlik el a valóságban. A szerviztábla azt mondja, egy kód "főzőegység-hiba"; a fórum azt, hogy az ön modelljén ez rendszerint csak egy beszorult kávétorta és negyedóra tisztítás. A szálakat bizonyítékként kezelje, nem igazságként:

- Súlyt kapjon az a bejegyzés, amely pontosan az ön modelljét nevezi meg, és hetekkel később is tartó javítást ír le.
- Ne bízzon olyan szálban, amelyik minden kódra, minden gépen ugyanazt az alkatrészt ajánlja.
- Ha a fórum és a szervizdokumentum ellentmond egymásnak: jelentésben a dokumentum, valószínűségben a fórum győz.

## A csapda: ugyanaz a kód, más jelentés

Itt rontja el a legtöbb öndiagnózis, mert a hibakódok nincsenek szabványosítva — márkák között sem, néha egy márka saját termékkínálatán belül sem.

- Ugyanaz a szám egymástól független dolgot jelenthet. Jurán az Error 2 a kávetermoblokk érzékelőkörének hibája — vagy csak a gép túl hideg a fűtéshez. Philipsen vagy Saecón az Error 02 belső hiba, amely egyenesen a szervizhez irányít. Ugyanaz a szám, hasonló kategória, más alrendszer és más számla.
- A szavak mögött kód rejtőzhet: a De'Longhi General Alarmnak számos ikerkódja van, amelyet a technikusok látnak; a jó javításhoz mindkét réteget ismerni kell.
- A gépkategória legalább olyan fontos, mint a márka: egy kódkarakter a tűzhelyen egészen mást jelent ugyanazon márka mosogatógépén. Először géptípusra szűrjön, és csak utána modellre.

Vesse össze a jelentést a tünettel: fűtéskód egy gépen, amely még mindig melegít, vagy leeresztéskód egy gépen, amely rendesen leereszt — többnyire azt jelenti, hogy rossz bejegyzést olvas, vagy a rossz modellhez.

## Ötlépéses ellenőrző lista

- Fotózza le a kijelzőt, és írja le a jelzőtáblán lévő teljes típusszámot.

- Szerezze meg a gyártó jelentését a kézikönyvből vagy a szervizdokumentációból.

- Erősítse meg legalább két olyan fórumtémával, amely az ön modelljét nevezi meg, és tartós javítást ír le.

- Nézze utána egy független referencialapon is: a [Philips Error 11 vagy 19](https://hu.codefixcoffee.com/philips-saeco/espresso-machines/error-11-or-19) jelentésének minden forráson ugyanaznak kell lennie; ha két forrás eltér, azt higgye, amelyik szervizdokumentációra hivatkozik.

- Állítsa vissza a gépet egyszer, majd döntsön: ha a kód azonnal visszatér, valós hiba — válasszon az olcsó alkatrész, a tisztítás és a szerelő között.

## Mikor hagyja abba a kutatást

Zárja be a fület, amikor két egymástól független forrás egyetért a jelentésben, és a tünet is passzol hozzá. További olvasással már nem változtat meg semmit egy kód, amely visszaállítás után azonnal visszatér — innentől a döntés tisztán gyakorlati: az alkatrész ára a gép korához és értékéhez mérve.

### Magyar vonatkozás

Magyarországon sok gép uniós webshopból érkezik, és a dobozában gyakran nincs magyar nyelvű használati utasítás — a típuspontos dokumentum a gyártó hivatalos oldaláról tölthető le a jelzőtáblán található típusszámmal. A fórumozásnál érdemes a magyar témák mellett az angol és német szálakat is elolvasni, mert a gyári kódtáblázatok ott jellemzően teljesebbek. A jelzőtábla egyébként a gép ajtószélén, a belső falán vagy a hátlapján szokott lenni.
