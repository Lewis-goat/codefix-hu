---
title: "De'Longhi General Alarm: mit jelent valójában"
description: "A General Alarm a De'Longhi gyűjtőhibája, rejtett kódként 1101 vagy 1512. Mit takar leggyakrabban, a tízperces infúzor-művelet, és mikor állj le."
---

A Magnifica, Dinamica vagy PrimaDonna kijelzőjén a General Alarm tűnik a legijesztőbbnek, pedig a legkevesebbet árulja el magából — és ez nem véletlen. A De'Longhi gépek többsége hibakódok helyett szöveges üzeneteket mutat: inkább közli, milyen típusú gondot észlelt, minthogy egy szerviztáblázatba való számot dobjon fel. A háttérben ugyanakkor az újabb modellek numerikus kódot is naplóznak — 1101, 1454, 2257 és társai —, amelyeket a szerviz akkor olvas ki, ha a gép asztalra kerül. Nálunk minden De'Longhi oldalon megtalálod mindkét réteget, a szöveget és a rejtett számot egyaránt; a sort a [General Alarm (1101 / 1512) kódos oldal](https://hu.codefixcoffee.com/delonghi/magnifica-dinamica/general-alarm-code-1101-1512/) nyitja.

## Gyűjtőhiba, nem diagnózis

A General Alarm lényege, hogy a vezérlőelektronika hibát észlelt, de nem tudja behatárolni, melyik alkatrész a felelős. Ott, ahol a gép számokat is mutat, 1101-es vagy 1512-es kódként kerül a rejtett naplóba. Ez a numerikus napló máshol pontosabb is lehet — a 1454 például a daráló blokkolódásának kódja —, de a General Alarm szándékosan tág, a kijelző pedig szándékosan homályos marad.

A gyakorlatban ECAM és ESAM gépeken tízesből kilencszer az **infúzor** — a kivehető főzőegység — a ludas. Elakadt, koszos vagy tisztítás után rosszul visszaigazított, esetleg kávépor ülepedett arra a kis optikai érzékelőre, amely a helyzetét figyeli. A második leggyakoribb ok a vízkör mészköve, ami miatt a szivattyúnak erőlködnie kell — a vezérlőelektronika ezt is általános hibaként jelenti, nem pontosként.

A homályban rejlik a jó hír: a General Alarm túlnyomó többsége tíz perc alatt, ingyen orvosolható.

### A tízperces rutin

1. Kapcsold ki a gépet a hátsó kapcsolóval, várj 30 másodpercet, majd kapcsolj vissza. Egy egyszeri elektronikus hiba itt magától elszáll.
2. Nyisd ki a szervizajtót, nyomd be a két piros gombot, és húzd ki az infúzort.
3. Öblítsd folyó víz alatt — szappan nélkül —, közben mozgasd meg kézzel a dugattyút, végül hagyd megszáradni.
4. Nézz bele az üregbe, ahonnan az infúzor kijött: egy kis érzékelőablak van ott, egy száraz ronggyal töröld le róla a kávéport.
5. Helyezd vissza az infúzort kattanásig, a karját teljesen lenyomva, majd zárd az ajtót, és indítsd újra a gépet.

### Ha visszajön a riasztás

Futtass le egy mészetlenítési ciklust. A meszesedett vízkör akkor is riaszt, ha az infúzor makulátlan, és évesnél idősebb gépeken a mészetlenítés több esetben megoldás, mintsem nem. Ha az infúzor kézzel sem mozdul, vagy repedt tömítést látsz rajta, ne állj tovább bíbelődni: cseréld ki. A szerelvény a típustól függően 7313251451 vagy 7313251441 számú kit, és a csere öt perces munka.

## Miért szavakat jelenít meg a De'Longhi, nem kódokat

A kijelző filozófiája egyszerű: a szó cselekvésre ösztönöz, a szám keresésre késztet. Egy „1101”-en szolgáltatási táblázat nélkül nem tudsz mit kezdeni, a „General Alarm” viszont legalább arra figyelmeztet, hogy állj meg és nézz körül. A rejtett numerikus réteg a táblázattal rendelkező szerelőnek készült — ezért vezetjük fel mi is mindkettőt minden oldalra, hogy ne kelljen választanod.

A többi De'Longhi üzenet ugyanennek a logikának engedelmeskedik: mindegyik megnevezi, milyen cselekvést vár tőled a gép. A [Water Circuit Empty / Fill Circuit](https://hu.codefixcoffee.com/delonghi/magnifica-dinamica/water-circuit-empty-fill-circuit/) akkor jelenik meg, amikor levegő került a szivattyúba, és az nem tud feltöltődni. Az [Insert Grounds Container](https://hu.codefixcoffee.com/delonghi/magnifica-dinamica/insert-grounds-container-empty-grounds-container/) mögött gyakran csak annyi áll, hogy a tartó mögötti érintkezők a nedves kávészutat hiányzó tartóként értelmezik. Ezek sem pontos alkatrész-diagnózisok — inkább utasítások.

Aki az ellenkező szemléletet keresi, nézze meg a Nespressót: a Vertuo gépek a hibák többségét villogó fénymintákkal jelzik szavak helyett, nem véletlenül készült hozzájuk [fényminta-fordító](https://hu.codefixcoffee.com/nespresso/vertuo-machines/blinking-lights/). A De'Longhi megközelítése és a teljes üzenetcsalád a [De'Longhi összefoglaló oldalon](https://hu.codefixcoffee.com/delonghi/) található. Ha a használati utasításra vagy a gyári dokumentációra van szükséged, a [De'Longhi hivatalos támogatási oldala](https://www.delonghi.com) jó kiindulópont.

## Mibe kerül

- A legtöbb esetben semmibe: az öblítés, az érzékelő letörlése és egy újraindítás megoldja.
- Mészetlenítő folyadék, ha a meszesedés a kiváltó ok: körülbelül 10 €.
- Csere infúzor-szerelvény, ha a meglévő repedt vagy beragadt: 35–60 €.
- Garancián kívüli gyártói szervizelés szuperautomata gépen: jellemzően 250–500 €, visszaszállítással; egy alkatrészes hibánál a független kávégép-javítók általában olcsóbbak.

### Amit itthon érdemes tudni

A magyar csapvíz túlnyomórészt kemény, magasabb kalciumtartalommal, ezért a meszesedésre visszavezethető General Alarm itthon hamarabb jelentkezhet, mint lágyvizes országokban. Érdemes a mészetlenítést a gyári intervallumnál sűrűbbre venni, nagyjából két-háromhavonta, vagy a tartályba palackozott, lágy vizet tölteni. A gyári mészetlenítő folyadék a nagyobb hazai webshopokban és márkaszervizekben egyaránt beszerezhető.

A General Alarm tehát nem halálos ítélet. A gép azt vallja be vele, hogy nem tudja pontosan, mi romlott el — és tízesből kilencszer egy tiszta infúzor meg egy letörölt érzékelő jelenti a teljes választ. Kezdd a fenti rutinnal, haladj sorban, és csak akkor gondolkozz alkatrészen vagy szervizen, ha a riasztás túlélte az öblítést és a mészetlenítést is.
