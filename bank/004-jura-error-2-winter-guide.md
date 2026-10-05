---
title: Jura Error 2 télen: a hideg gép mint ok, amiről kevesen beszélnek
description: A Jura Error 2 sokszor nem alkatrészhiba: 10 °C alatt a vezérlő letiltja a fűtést. Bemelegítési protokoll, és mikor valóban az NTC hőérzékelő a hibás.
---

Az Error 2 a leggyakoribb kód a Jura automata gépeken — az E, ENA, S, J, Z és GIGA sorozatok ugyanazt a számozást használják —, és két nagyon különböző arca van. Vagy a kávetermoblokk hőérzékelőjének köre szakadt meg, vagy a gép egyszerűen túl hideg a fűtéshez. Télen ez a második eset ejti csapdába a meglepően sok olyan tulajdonost, aki mindent jól csinált — és erre a hibaüzenet egy szóval sem utal. A teljes referencia a [Jura Error 2 oldalon](https://hu.codefixcoffee.com/jura/automatic-machines/error-2); ez a cikk a történet hideg felével foglalkozik.

## Mit mond valójában a gép

A Jura 1–5 közötti hibái mind a termoblokk fűtéséhez és érzékelőihez kapcsolódnak. Amikor az elektronika olyan hőmérsékleti értéket lát, amelyet nem tud összeegyeztetni az elrendelt fűtéssel, lekapcsolja a fűtést, és nem próbálkozik újra — ez védelmi lezárás, nem feltétlenül meghibásodás. Körülbelül 10 °C alatt egy hideg termoblokk messze a várt tartományon kívül van, és a vezérlő pontosan úgy kezeli, mintha a hőérzékelő hibás lenne. Semmi nem tört el. A gép hideg.

A helyzet klasszikus: télen futárral érkezett gép egy fűtetlen rakodótér után; a Jura hideg konyhában, télikertben, garázsban irodázik vagy a nyaralóban áll; esetleg most bontották ki, és azonnal bekapcsolták. A minta mindig ugyanaz — korábban rendben működött, az Error 2 az első indításkor jelenik meg, és semmi lenyomás nem tünteti el.

A kávégépek egyébként sem szeretik a hideg indítást. A Philips és Saeco gépeknek megvan a maga párja: az Error 11 vagy 19 azt jelenti, hogy a gépnek hideg szállítás után előbb szobahőmérsékletre kell kerülnie — ezt részletezi a [Philips Error 11 vagy 19 oldal](https://hu.codefixcoffee.com/philips-saeco/espresso-machines/error-11-or-19).

## A bemelegítési protokoll

Futtassa le, mielőtt bármit elhibásítana. Nem kerül semmibe, és hideg gépnél mindig ez az első lépés.

- Vigye a gépet fűtött szobába, és adjon neki időt — több órát, hogy valóban szobahőmérsékletű legyen, ne csak kézzel kevésbé hidegnek tűnjön. Egy látszólag rendben lévő vázban is ülhet a termoblokk 10 °C alatt.

- Gyorsításként fújjon hajszárítót a legalacsonyabb fokozaton a víztartály üregébe öt percen keresztül, vagy töltse fel a tartályt langyos — nem forró — csapvízzel.

- Indítsa újra a gépet.

- Ha az Error 2 a bemelegedés után eltűnik, semmi nem hibásodott meg. Tartsa a gépet melegebb helyen, és a kód nem tér vissza.

Két óvatosság. A langyos víz langyos legyen, ne forró: a tartály, a szelepek és a tömítések műanyagból vannak. És ne irányítson sűrített meleget a gép testére vagy elektronikájára — a cél a termoblokk lehűtésének megszüntetése, nem a környező vezetékek megfőzése.

## Mikor valóban az NTC hőérzékelő vagy a hőbiztosíték-vezetékek hibája

Ha a gép valóban felmelegedett — órákig állt fűtött szobában —, és az Error 2 mégis jelentkezik, a jóindulatú magyarázat elfogyott, az érzékelőkör szakadt. Egy Jurán belül ez két leletet jelent:

- A kávetermoblokk NTC hőérzékelője hibásodott meg, vagy a csatlakozója vesztette el a kontaktot. A testvérkód a [Jura Error 1](https://hu.codefixcoffee.com/jura/automatic-machines/error-1), a kávetermoblokk érzékelőhibája szűkebb értelemben; a kettő alkatrészben és tünetekben rokon.

- A termoblokkot védő két hőbiztosíték-vezeték szakadt meg — túlmelegedés után vagy egyszerűen korral. A szakadt vezeték multimméteren nyitott kört mutat.

A javítás többnyire megéri. Egy gyári Jura NTC hőérzékelő kb. 25–40 €, a hőbiztosíték-vezetékek szettje 15–30 €; a technikusok általában együtt cserélik a kettőt, mert a munka ugyanannyi. Még egy teljes termoblokk is, 90–180 €-ért, kifizethető lehet a felső kategóriás gépeken. Ha az ön Jura-jának végig meleg volt a környezete, akkor ez — nem az időjárás — az ön Error 2-je.

## A javítás utáni figyelmeztető jel

Egy csapda megérdemel egy saját bekezdést. A hőbiztosíték-vezeték, amely egyszer átégett, újra kiég, ha a tápelektronika beragadva tartja a fűtést. Ha az újonnan beszerelt vezeték napokon belül újra hibázik, ne cseréljen további biztosítékot: a hiba a tápon van. Egy alap jellemzően 120–250 € munkadíj nélkül, ami idősebb gépnél már inkább ajánlat-versus-új gép beszélgetés, mintsem alkatrészrendelés.

## Biztonság és határok

A Jura kinyitása nem a vízforraló kinyitása. A ház ovális fejű Torx-Plus biztonsági csavarokkal van összeszerelve, a termoblokkok hálózati feszültséget vezetnek, a gyári dokumentumokért pedig a [Jura hivatalos weboldala](https://www.jura.com) a kiindulópont. Ha nincs meg a megfelelő csavarozó, a mérőműszer és a hálózati feszültség melletti rutin, ez már műhelymunka — szakemberre való. A bemelegítési protokoll az Error 2 felhasználói fele; a hőérzékelő és a biztosítékvezetékek a műhely fele.

A gazdaság mindkét irányban barátságos. A bemelegítés nem kerül semmibe, az érzékelő és hőbiztosíték-vezeték javításának reális alkatrészszámlája pedig 50 € alatt marad. A márka többi kódjához — a szelep-, főzőegység- és fűtéskódokhoz minden modellsorozaton — induljon a [Jura áttekintő oldalról](https://hu.codefixcoffee.com/jura). Ha más kávégép is van a házban: a Miele CM és CVA rendszerek F-számú kódsémát használnak, amelyet a [Miele áttekintésünk](https://hu.codefixcoffee.com/miele) indexel, a gyártó saját oldala ([Miele](https://www.miele.com)) pedig jó kiindulópont a dokumentumokhoz.

### Magyarországon télen

Magyarországon különösen a nyaralókban és hétvégi házakban álló gépeket érinti a jelenség: októbertől áprilisig a fűtetlen épületben a gép belseje tartósan 10 °C alatt marad, és az Error 2 jellemzően az első tavaszi indításnál jelentkezik. Hasonló a helyzet a fűtetlen garázsban vagy kamrában tartott gépekkel, valamint a télen, futárral érkezett csomagokkal is. Bontás előtt a gépet mindig hagyja egy éjszakán át fűtött szobában felmelegedni.
