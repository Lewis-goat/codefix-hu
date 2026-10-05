---
title: "Miele F77: a szelepek inicializálásakor jelentkező hibakód"
description: "A Miele F77 belső hibát jelez a szelepek inicializálásakor CM és CVA gépeken. Először áramtalanítás; visszatérő kódnál szerviz."
---

A Miele kávégépek szokatlanul őszintén bánnak a saját hibáikkal: a beépített öndiagnosztika F-kódjainak jelentését még a használati utasításban is kinyomtatják. Közülük az F77 az, amellyel senki sem szeretne találkozni. A kód lényege egy **induláskor észlelt belső meghibásodás**, a gyakorlatban leggyakrabban a gépen belüli vízutakat kapcsoló szeleprendszer inicializálási hibája, és a Miele táblázatának komoly végén tanyázik. Pulton álló CM gépeken (CM 5510, CM 6150) és beépített CVA egységeken (CVA 6401, CVA 6805) egyaránt előfordul, kissé eltérő megfogalmazással. A [részletes F77 hibaoldal](https://hu.codefixcoffee.com/miele/cm-cva-machines/f77/) a javítási részleteket tárgyalja; ebben a bejegyzésben azt járjuk körbe, mit jelent az inicializálás, és meddig mehet el a tulajdonos a saját eszközeivel.

## Mit jelent valójában az inicializálás

Egy Miele kávégép bekapcsoláskor nem egyszerűen felmelegszik, aztán vár. A vezérlőelektronika minden egyes bekapcsolásnál végigfuttat egy indítási szekvenciát, és még az első ital felajánlása előtt ellenőrzi, hogy a belső alkatrészek a várt módon válaszolnak-e. Az F77 pontosan ide, a szekvencia közben kerül naplózásra: az elektronika belső hibát észlelt a gép indulása alatt, a legtöbb esetben a vizet a gépen belül irányító szeleprendszer érintettségével. A kézikönyv szándékosan tág megfogalmazása („belső hiba”) miatt ugyanaz a szám jelölhet szelep-, szivattyú- vagy vezérlőelektronika-meghibásodást is.

Éppen ez a szélesség választja el az F77-et a Miele barátságosabb kódjaitól. Az [F10 és F17](https://hu.codefixcoffee.com/miele/cm-cva-machines/f10-f17/) lényege, hogy a gép vizet akart szívni, és nem sikerült: üres, rosszul behelyezett vagy beragadó kivehető víztartály CM gépeknél, zárt vízelzáró vagy eltömődött szűrő a vezetékes CVA kiviteleknél. Ezek valóban a felhasználóra bízott javítások. Az F77 ezzel szemben magas súlyosságú, önjavításra nem javasolt kód, és a kézikönyv által felajánlott egyetlen teendő az áramtalanítás.

## Az első teendő: az áramtalanítás, amit maga a Miele javasol

A hivatalos útmutató őszintén megmondja, meddig terjed az önkiszolgálás — mégis érdemes rendesen, a végéig elvégezni, mielőtt bármi másba fogna az ember:

1. Kapcsolja ki a gépet a be-/kikapcsoló érintőszenzorral, ne csak készenléti állapotban hagyja.
1. Húzza ki a hálózati dugaszt a fali aljzatból.
1. Várjon több percig. Ha az F77 korábban rövid kikapcsolás után már visszatért, adjon neki egy teljes órát — több Miele kézikönyv pontosan ezt az időt javasolja.
1. Dugja vissza, kapcsolja be, és figyeljen egyetlen dologra: a hiba azonnal, az inicializálás közben jelenik-e meg, vagy csak később, egy ital lekérésekor.

Ez az időzítés a leghasznosabb megfigyelés. Az az F77, amely eltűnik és soha többé nem tér vissza, átmeneti volt, és az áramtalanítás önmagában jelentette a teljes javítást. Az az F77 viszont, amely azonnal, minden alkalommal, az indítási szekvencia ugyanazon pontján tér vissza, azt üzeni, hogy egy alkatrész bukik meg az ellenőrzésen — nem pedig az elektronika zavarodott össze egyetlen egyszeri alkalommal. Jegyezze fel, mit látott, mielőtt bárkit felhív.

## Mikor van szükség valóban Miele szervizre

Ha az áramtalanítás nem hoz tartós eredményt, a reális okok a szelepegység, a szivattyú vagy a vezérlőelektronika közül kerülnek ki — ez utóbbi a három közül a legköltségesebb. Ilyenkor a helyes lépés a megállás és a gép átadása:

- **Ne vegye le a külső burkolatot.** A Miele kifejezetten rögzíti, hogy a házat nem szabad eltávolítani: a gép belső feszültségeket és nyomás alatt álló vízrendszert rejt. Ez a figyelmeztetés pontosan ilyen jellegű hibákra vonatkozik.
- **Hívás előtt jegyezze fel a típusszámot.** A CM 5510/6150 és a CVA 6401/6805 gépek belső felépítésben különböznek, és ha pontosan tudja, melyik van a konyhában, a diagnosztika gyorsabban halad.
- **Alkatrészszintű árajánlatra számítson, ne homályos összegre.** Egy szelepegység nagyjából €50 és €120 közé esik; a vezérlőelektronika ezt jóval meghaladja. Garancián kívüli gyári szervizelés egy szuperautomatánál jellemzően €250–€500, a visszaszállítással együtt, a független kávégépjavítók pedig az egy alkatrészt igénylő munkáknál általában olcsóbbak.

Ez az ársáv azt is megmagyarázza, miért éri meg az F77-t javítani a csere helyett: a CM és CVA rendszerek annyiba kerülnek, hogy még a szervizi sáv felső vége is ésszerű egy új beépített géppel szemben — az eldöntő áramtalanítási kísérlet pedig nem kerül semmibe.

### Praktikus tanácsok magyarországi géptulajdonosoknak

A Miele Magyarországon hivatalos szervizhálózattal rendelkezik, a beépített CVA gépeknél helyszíni kiszállással is; az elérhetőségeket a [Miele hivatalos weboldala](https://miele.com) és a magyar képviselet ügyfélszolgálata adja meg. A hívás előtt jegyezze fel a gép adattábláján lévő típust és a hozzá tartozó Typed számot, mert enélkül a szerviz nem tud pontos alkatrészt rendelni. Ha a gép még jótállás alatt áll, a ház felnyitása a jótállás elvesztésével járhat, ezért az F77-nél különösen fontos a burkolatot érintetlenül hagyni.

## Az F77 helye a nagyobb képben

A teljes [Miele kódtáblázatban](https://hu.codefixcoffee.com/miele/) a minta következetes: a vízellátási kódokat a tulajdonos a mosogató mellett megjavíthatja, a szelepes és főzőegységes kódok a Miele szervizé tartoznak, és az F77 a második csoport legvilágosabb példája. Ha mellettük egy Sage vagy Breville gép is dolgozik a konyhában, annak kódjai egészen másként működnek — egy olyan szerviztáblából jönnek, amelyet a gyártó egyáltalán nem publikál; ezt boncolgatja a [Breville és Sage útmutatónk](https://hu.codefixcoffee.com/breville/).
