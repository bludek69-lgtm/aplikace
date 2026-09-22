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

### 1.2.8 (beta)
- Rozsah B: Jednoduché ověření jako pomocník s návrhy identity a podmíněnými cenovými podklady. Přesné ocenění konkrétní fotografie NENÍ prokázáno (0 z 20 živých ověření) — proto beta.
- Odhad AI (zoubkování, zkusmý tisk, forma vydání, stav lepu) se nevydává za doložený stav; správnou variantu už tvrdě nevylučuje. Doložit ho může jen měření okraje (jen přítomnost zoubkování) nebo pozorování rubu.
- Chybné katalogové číslo od AI aplikace odmítne podle nominálu a sama navrhne kandidáty podle viditelných znaků — i u známek bez vytištěné jednotky.
- Bez doloženého stavu lepu ukáže podmíněné cenové scénáře podle stavu z prodejů téhož čísla — nejsou to ocenění vašeho kusu.
- Tokeny a cena: odhad z tokenů × ceník, není to faktura Google. Zabalená aplikace nově obsahuje modul hledání podle znaků (v 1.2.7 chyběl).
- Nemění se: posudek je předběžné vizuální posouzení, není oficiální expertíza ani ověření pravosti; kalibrace pravosti neproběhla.

### 1.2.7
- Jednoduché ověření si samo dohledá podklady: referenční záznamy variant (Smithsonian — National Postal Museum) a skutečné prodeje z oficiálních výsledků aukcí (Burda Auction).
- Cena jen doložená prodeji téže známky ve stejném stavu; jinak srozumitelný důvod a jeden další krok. Odhad AI je jen označený jako nedoložený.
- Shoda fotografie s variantou vyžaduje viditelné rozlišovací znaky; podklady ukazují kandidáty, záměny a co je vylučuje.
- Jednodušší první krok: stačí fotka líce, odborné údaje jsou nepovinné; průběh ověření a tlačítko Zrušit.
- Nemění se: posudek je předběžné vizuální posouzení, není oficiální expertíza; kalibrace pravosti neproběhla.

### 1.2.6
- Nová stránka Jednoduché ověření: nahraješ líc a rub, aplikace zkontroluje kvalitu skenu, vybereš model Gemini a spustí se všech 14 kontrol — včetně tvých master promptů (identifikace, stav a pravost, tržní ocenění, obchodní rozbor) a hledání na internetu.
- Výstupní zpráva: identifikace, orientační cena, úroveň podezření na pravost (nikdy procento), stav, tabulka použitých kontrol, internetové zdroje, export do PDF a DOCX.
- Tokeny a cena ověření: skutečné tokeny × oficiální ceník Google podle modelu (USD i Kč), odhad už před spuštěním.
- Placený režim jen s klíčem a povolenými placenými voláními; jinak bezplatná simulace, která do Googlu nic nepošle.
- Vypnutý model Gemini 2.0 Flash a řada 1.5 zmizely z výběru modelů v celé aplikaci; nejlevnější volbou je nově Gemini 2.5 Flash-Lite.
- Nemění se: posudek je předběžné vizuální posouzení, není oficiální expertíza; kalibrace pravosti neproběhla (0 pravých vzorků).

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
