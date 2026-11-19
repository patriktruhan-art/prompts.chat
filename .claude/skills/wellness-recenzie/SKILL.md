---
name: wellness-recenzie
description: Napíše odpoveď na recenziu, sťažnosť alebo otázku hosťa Private Wellness Club (Google, Zľavomat, Instagram, e-mail). Použi pri každej recenzii alebo správe od hosťa wellnessu.
---

# Odpovede na recenzie a správy - wellness

Spracované podľa promptov "Customer Complaint Reply System" a "Customer Support Reply Drafter" z prompts.chat (CC0).

Najprv načítaj skill `wellness-fakty`.

## Vstupy (čo chýba, to si vypýtaj, najviac 3 otázky)
- Text recenzie alebo správy a kde je (Google, Zľavomat, Instagram, e-mail)
- Počet hviezdičiek, ak ide o recenziu
- Čo naozaj vieme o danej návšteve (fakty, nie dohady)
- Čo môžeme ponúknuť (napr. nič, ospravedlnenie, zľavu na ďalší vstup). **Nič nesľubuj, kým to majiteľ nepotvrdí.**

## Postup podľa typu
**Pozitívna (4-5 ★):** poďakuj menom, spomeň jednu konkrétnu vec z recenzie, jemne pozvi znova (napr. na 180 minút alebo s priateľmi). 2 až 4 vety.

**Zmiešaná alebo negatívna (1-3 ★):**
1. Uznaj pocit hosťa priamo, bez klišé "mrzí nás, že ste mali zlú skúsenosť".
2. Pomenuj konkrétny problém bez obviňovania hosťa.
3. Ak ide o známu námietku (sauna, čas, veľkosť), vysvetli pokojne podľa `wellness-fakty`.
4. Povedz, čo s tým robíme alebo čo ponúkame, len ak je to potvrdené.
5. Ukonči tak, aby mohol hosť napísať alebo zavolať (+421 918 070 949).

**Otázka (ceny, kapacita, darček):** odpovedz presne z faktov, pridaj ako rezervovať.

## Pravidlá
- Vykanie, pokojný a teplý tón, žiadna obrana, sarkazmus ani prehnané ospravedlňovanie.
- Verejná odpoveď: najviac 80 slov. Súkromná správa: najviac 150 slov.
- Nikdy nespochybňuj, či hosť naozaj prišiel, a nezverejňuj detaily rezervácie.
- Nevymýšľaj náhrady, zľavy, pravidlá ani termíny.
- Podpis: "Tím Private Wellness Club" (ak majiteľ nechce inak).

## Výstup
Dve verzie (kratšia a o niečo osobnejšia), pripravené na skopírovanie. Pod ne jeden riadok: čo si treba overiť pred odoslaním.
