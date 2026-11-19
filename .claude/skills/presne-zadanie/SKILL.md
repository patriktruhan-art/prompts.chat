---
name: presne-zadanie
description: Z hrubého nápadu spraví presné zadanie (prompt), aby AI urobila presne to, čo chceš. Použi, keď je požiadavka nejasná alebo keď chceš prompt, ktorý budeš používať opakovane. Pre Shopu aj wellness.
---

# Presné zadanie

Spracované podľa promptov "TCRE Framework", "Meta-Prompt Engineer" a "Prompt Enhancer (concise)" z prompts.chat (CC0).

## Postup
1. Zopakuj zadanie jednou vetou vlastnými slovami.
2. Zisti, či ide o Shopu, alebo o wellness. Načítaj príslušný skill `shopa-fakty` alebo `wellness-fakty` a nepýtaj sa na to, čo už v ňom je.
3. Polož najviac 4 otázky naraz, len tie, bez ktorých to nejde. Zisti hlavne:
   - **Úloha:** čo presne má vzniknúť (text, tabuľka, výpočet, scenár)?
   - **Kontext:** pre koho to je a kde sa to použije (Instagram, Google recenzia, Zľavomat, interne)?
   - **Vzor:** máš príklad, ktorý sa ti páči alebo nepáči?
   - **Hotové, keď:** dĺžka, formát a čo tam nesmie byť.
4. Keď máš odpovede, napíš finálne zadanie v tomto tvare:

```
ÚLOHA: ...
KONTEXT: ...
VSTUPY: ...
VÝSTUP: formát, dĺžka, jazyk, tón
PRAVIDLÁ: čo nesmie byť, čo si nevymýšľať
HOTOVÉ, KEĎ: ...
```

5. Krátko skontroluj zadanie: chýba úloha, kontext, vzor alebo merateľný cieľ? Navrhni najviac 2 vylepšenia.
6. Spýtaj sa, či ho rovno vykonať.

## Rýchly režim
Ak používateľ napíše "rýchlo" alebo "bez otázok", nič sa nepýtaj. Prepíš zadanie čo najstručnejšie a najpresnejšie, chýbajúce údaje označ {{doplniť}} a vypíš iba hotové zadanie.
