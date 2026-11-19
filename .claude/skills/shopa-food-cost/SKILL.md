---
name: shopa-food-cost
description: Vypočíta, koľko Shopu stojí porcia burgra, wrapu alebo prílohy, food cost v %, maržu a odporúčanú cenu; roztriedi menu na ťahúne a slabé položky. Použi pri otázkach "koľko ma stojí burger", "ako naceniť menu", "prečo mám vysoký food cost".
---

# Food cost a nacenenie menu - Shopa

Spracované podľa promptu "Menu Food Cost and Pricing Calculator" z prompts.chat (CC0).

Najprv načítaj skill `shopa-fakty` (aktuálne predajné ceny).

## Vstupy (vypýtaj si, čo chýba)
1. Receptúra jednej porcie: každá surovina a množstvo (g, ml, ks).
2. Nákupná cena suroviny a balenie (napr. hovädzie 1 kg = 11,90 € bez DPH).
3. Výťažnosť/odpad, ak je (orezávanie, vyprážanie, zmenšenie mäsa pri pečení). Ak ju nepoznáš, spýtaj sa, odhad označ ako odhad.
4. Obal pri rozvoze (krabička, papier, taška) a provízia Bistro.sk, ak ide o rozvoz.
5. Cieľový food cost (ak ho nemá, navrhni rozsah 28 až 35 % a povedz prečo).
6. Pre menu analýzu: počet predaných kusov za obdobie pri každej položke.

## Výpočet (vždy ukáž postup)
- Cena suroviny na porciu = nákupná cena ÷ množstvo v balení × množstvo v porcii ÷ výťažnosť
- Náklad na porciu = súčet surovín + obal (pri rozvoze)
- Cena bez DPH = predajná cena ÷ (1 + sadzba DPH). **Sadzbu DPH pre jedlo a nápoje si vypýtaj alebo over, nehádaj.**
- Food cost % = náklad na porciu ÷ cena bez DPH × 100
- Marža v € = cena bez DPH − náklad na porciu
- Odporúčaná cena = náklad ÷ cieľový food cost × (1 + DPH), zaokrúhlená na x,40 / x,90 ako zvyšok menu

Výpočty rob v kóde alebo v tabuľke, nie z hlavy.

## Analýza menu (keď máš predaje)
Rozdeľ položky podľa popularity a marže v €:
- **Hviezda** (predáva sa, zarába): nechať, zviditeľniť.
- **Ťahúň** (predáva sa, zarába málo): jemne zdražiť alebo upraviť porciu, nie kvalitu.
- **Záhada** (zarába, málo sa predáva): lepšia fotka, popis, umiestnenie, reel.
- **Slabá** (málo sa predáva, málo zarába): zvážiť zmenu alebo vyradenie.

## Výstup
1. Tabuľka: položka · náklad · cena bez DPH · food cost % · marža € · odporúčanie.
2. 3 najdôležitejšie kroky, zoradené podľa toho, koľko € prinesú.
3. Riadok "Čo je odhad": všetky predpoklady.

## Pravidlá
- "Na surovinách nešetríme" je základ Shopy: nikdy neodporúčaj lacnejšie suroviny na úkor kvality ako prvú voľbu. Najprv cena, porcia, odpad, nákupné podmienky.
- Myslí sa na maržu v €, nie len na percentá.
- Nevymýšľaj nákupné ceny ani predaje.
