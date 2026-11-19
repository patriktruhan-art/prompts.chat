---
name: shopa-alergeny
description: Zostaví tabuľku 14 alergénov EÚ pre menu Shopy z receptúr, upozorní na skryté alergény a krížovú kontamináciu a pripraví odpovede pre personál. Použi pri alergénoch, novom jedle alebo otázke hosťa na alergiu.
---

# Alergény v menu - Shopa

Spracované podľa promptu "Restaurant Menu Allergen Matrix Builder" z prompts.chat (CC0).

Najprv načítaj skill `shopa-fakty` (zoznam jedál).

## 14 alergénov EÚ (číslovanie podľa slovenskej praxe)
1 obilniny s lepkom · 2 kôrovce · 3 vajcia · 4 ryby · 5 arašidy · 6 sója · 7 mlieko · 8 orechy · 9 zeler · 10 horčica · 11 sezam · 12 oxid siričitý a siričitany · 13 vlčí bôb · 14 mäkkýše

## Vstupy
- Každé jedlo so všetkými zložkami: žemľa, mäso, syr, omáčky, zelenina, posyp, olej na vyprážanie.
- Značkové polotovary (žemle, omáčky, dresingy, koreniny, panko, tortilly) a čo píšu na etikete.
- Kuchyňa: spoločná fritéza? spoločný gril a dosky? kde sa robí veggie wrap?

## Postup
1. Pre každé jedlo prejdi každú zložku a priraď alergény iba podľa toho, čo je zadané.
2. Ak zložka chýba alebo etiketu nepoznáš, napíš "OVERIŤ", nie "bez alergénu".
3. Vypíš skryté zdroje, na ktoré sa zabúda: majonéza a omáčky (vajcia, horčica), sezam na žemli, panko a strúhanka (lepok), syry a maslo (mlieko), worcester (ryby), sušené paradajky a ocot (siričitany), korenistá zmes (zeler, horčica).
4. Krížová kontaminácia: spoločná fritéza, gril, nože, rukavice. Ak je riziko, uveď "môže obsahovať stopy".

## Výstup
1. Tabuľka: jedlo × 14 alergénov (✔ obsahuje · ~ stopy · ? overiť), pod tým čísla alergénov na menu, napr. "1, 3, 7, 10, 11".
2. Zoznam otázok na dodávateľov.
3. Odpovede pre personál (2 až 3 vety, tykanie s hosťom podľa štýlu Shopy), napr. keď hosť povie "mám alergiu na lepok".
4. Bezpečné náhrady, len ak existujú (napr. bezlepková žemľa, ak ju naozaj máte).

## Pravidlá
- **Nikdy netvrď, že jedlo je bez alergénu, ak to nevieš isto.** Pri vážnej alergii hosť musí dostať pravdivú odpoveď, aj keď je "nevieme isto".
- Tento výstup je pracovný podklad, finálne označenie skontroluje majiteľ podľa etikiet.
