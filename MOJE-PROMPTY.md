# Moje prompty - Shopa a Private Wellness Club

Vybrané prompty z tejto zbierky, preložené do slovenčiny a prispôsobené dvom podnikom. Sú uložené ako skills pre Claude Code v priečinku `.claude/skills/`.

## Ako ich používať
1. Otvor tento repozitár v Claude Code (claude.ai/code alebo v termináli príkazom `claude` v priečinku repozitára).
2. Napíš úlohu normálne ("odpovedz na túto recenziu na wellness: ..."), Claude si vhodný skill vyberie sám.
3. Alebo ho zavolaj priamo, napr. `/wellness-recenzie` alebo `/shopa-food-cost`.

## Zoznam
| Skill | Na čo |
|---|---|
| `presne-zadanie` | Z hrubého nápadu spraví presné zadanie (pre oba podniky) |
| `zdrazenie-cien` | Ako zdražiť bez straty zákazníkov (pre oba podniky) |
| `wellness-fakty` | Ceny, služby, tón a námietky wellnessu (načítava sa automaticky) |
| `wellness-recenzie` | Odpovede na recenzie a správy hostí |
| `wellness-instagram` | Reels, príspevky, popisy pre @privatewellnesspresov |
| `wellness-ponuka` | Balíky, darčekové poukazy, ponuky na zľavové portály |
| `shopa-fakty` | Menu, ceny, štýl Shopy (načítava sa automaticky) |
| `shopa-food-cost` | Koľko stojí porcia, food cost, nacenenie, analýza menu |
| `shopa-alergeny` | Tabuľka 14 alergénov, otázky na dodávateľov, odpovede personálu |
| `shopa-recenzie` | Odpovede na recenzie a sťažnosti v štýle Shopy |

Instagram pre Shopu riešia samostatné skills v Claude účte (shopa-ig-pravidla, shopa-ig-obsah, shopa-ig-komunita).

## Údržba
- Ceny wellnessu overené 19. 11. 2026, ceny Shopy 26. 10. 2026. Pri zmene uprav `wellness-fakty` alebo `shopa-fakty`.
- Wellness už neponúka ubytovanie (potvrdené 19. 11. 2026). Ak sa to zmení, uprav `wellness-fakty`.
