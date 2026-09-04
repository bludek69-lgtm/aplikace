# Změny v aplikacích

Stručný přehled uživatelských změn v aktuálních verzích. Detaily a starší verze najdeš
přímo v jednotlivých aplikacích.

## BudLine Panel

### 1.2.3
- Nová stránka „Co je nového“ + okno po aktualizaci — po updatu hned uvidíš, co přibylo nebo se opravilo.
- Uvítací průvodce se nově ukáže jen při prvním spuštění (ne při každém startu). Znovu ho otevřeš tlačítkem „?“.
- Výpočet mzdy a porovnání pásek zůstávají beze změny.

### 1.2.2
- Bezpečnostní rotace instalačního hesla (vlastní heslo jen pro tuto aplikaci).

### 1.2.1
- Zpevněný auto-update: přesná kontrola zdroje aktualizace + povinné ověření kontrolního součtu (SHA-256).
- Bezpečný ruční režim aktualizace, když není k dispozici instalační heslo.

## Meal Planner

### 0.8.4
- Bezpečnostní rotace instalačního hesla a zpevněný tichý auto-update.

## Italia Travel Planner

### 0.7.4
- Bezpečnostní rotace instalačního hesla a zpevněný auto-update.

## Collection

### 1.2.5
- Vlastní atestované známky: fotografie + atest nebo posudek, nejdřív lokální analýza (nic se nezapíše), pak uložení jako kandidát — ground truth vzniká jen po tvém schválení. Dávkový import z intake složky, originály se nemění.
- Pozměněné pravé známky (regumované, reperforované…) jako samostatná referenční třída mimo binární dataset pravý / padělek.
- Expertní autority BPP, SČF a VÖPh schválené vlastníkem (AIEP jen adresář); žádosti o práva k obrázkům se stavy SENT / READY FOR MANUAL SEND / GRANTED / PARTIALLY GRANTED / DENIED / UNCLEAR — odesláno nikdy neznamená povoleno.
- Zdraví knihovny: kandidáti vlastníka, práva, autority a pravdivé síťové účetnictví (aplikační HTTP / research web / ostatní / celkem).
- Nemění se: posudek je předběžné vizuální posouzení, není oficiální expertíza; kalibrace pravosti neproběhla (0 pravých vzorků, 18 padělků schválených vlastníkem).

### 1.2.4
- Kalibrace pravosti v Expertize je hotová od začátku do konce: stav datasetu, zdroje kalibračních dat, cílené hledání chybějících vzorků v oficiálním muzejním zdroji (jen volně licencované obrázky s výslovnou klasifikací), kandidáty schvaluješ ty po jednom, ruční vzorek s fotkou a atestem, prohlížeč datasetu.
- Nemění se: posudek je předběžné vizuální posouzení, ne certifikát pravosti; kalibrace pravosti neproběhla (ground truth = 0), stav se odvozuje z měření.


### 1.1.3
- Bezpečnostní rotace instalačního hesla a zpevněný auto-update.
