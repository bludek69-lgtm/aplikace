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

### 1.10.5 (beta)
- 1.10.5 BETA — Lepší diagnostický balíček. U každého ověření je nově vidět použitý model AI, režim (placený / simulace) a odpověď služby — např. HTTP 404 znamená, že model není pro tento účet dostupný (nový klíč Google: vyber model řady 3); kontrola „Poslední ověření“ rovnou poradí, co dělat. U série je souhrn známek (dokončeno / selhalo / nespuštěno). Doba běhu aplikace se měří správně (dřív to byl čas od otevření stránky Diagnostika), balíček nese pseudonymní otisk instalace (rozliší dva počítače bez jména PC a cest) a nastavené modely. Export po kliknutí potvrdí uložení, druhé kliknutí do 10 s ignoruje a soubor má v názvu datum a čas. Soukromí beze změny: žádné známky, ceny, fotky, prompty, klíče, jména ani cesty. NENÍ oficiální expertíza; kalibrace pravosti neproběhla.

### 1.10.4 (beta)
- 1.10.4 BETA — Novější modely Gemini. Google pouští nové účty (nový API klíč) jen k modelům řady 3; u řady 2.5 vrací chybu 404 „no longer available to new users“. Ve výběru modelu u placeného posudku, Jednoduchého ověření i na stránce Klíče & API jsou nově Gemini 3.8 Flash (nejnovější Flash, doporučený pro nové účty), Gemini 3.6 Flash a Gemini 3.1 Flash-Lite (nejlevnější z řady 3); na Klíče & API přibyl i 3.5 Flash-Lite. Ceny podle ceníku Google k 2026-10-13: 3.8 a 3.6 Flash 0,75 / 3,75 USD za 1 mil. tokenů do 31. 12. 2026, od 1. 1. 2027 1,50 / 7,50 — aplikace přepne cenu sama podle data; 3.1 Flash-Lite 0,25 / 1,50. Výchozí model se nemění (2.5 Pro). NENÍ oficiální expertíza; kalibrace pravosti neproběhla; živé volání nových modelů nebylo provedeno (ověřen jen 3.5 Flash-Lite).

### 1.10.3 (beta)
- 1.10.3 BETA — Oprava zacyklených odpovědí AI. Když model (hlavně Gemini 2.5 Flash) začne psát dokola totéž (řady nul, stále stejný řádek tabulky), aplikace opakování zkrátí a označí „[… odpověď se zacyklila, zkráceno …]“ — zpráva PDF/DOCX už nemá desítky stran nesmyslů, a to ani u dříve uložených ověření. Zacyklený a useknutý rozbor se jednou automaticky zopakuje (stejné brány rozpočtu a USD stropu; u 2.5 Flash nejvýše asi 0,10–0,12 USD navíc za rozbor) a použije se lepší odpověď. Cenový řádek, jehož popis odporuje katalogovému číslu nebo stavu (např. jiná série, ** proti razítkované), nebo jehož odkaz vede na výsledky hledání místo konkrétní položky, se do podmíněných cen nezapočítá. U archu je u každé ceny vidět, ke které známce patří (L3: …). NENÍ oficiální expertíza; kalibrace pravosti neproběhla; živý placený AI test této změny nebyl proveden.

### 1.10.2 (beta)
- 1.10.2 BETA — Zoubkoměr a přehlednější zpráva. Aplikace měří hodnotu zoubkování přímo ze skenu: najde každou dírku, z rozteče spočítá zuby na 2 cm a ukáže náhled změřených dírek. Bez kalibrace přibližně (±2 %, zápis na půlky, např. „≈ 14“, kombinované „≈ 13½ × 13“); po naskenování pravítka (Zoubkoměr — kalibrace pravítkem) ±0,05 a zápis na čtvrtky. Zpráva PDF/DOCX má klikací odkazy na zdroje, snímky známky (líc a rub) s popisem stavu u každé známky a u archu sekci Sada. U promptů a kontrol v kroku 3 je ikona ⓘ s vysvětlením, co dělají. Měření ze skenu není odborné potvrzení varianty; NENÍ oficiální expertíza; kalibrace pravosti neproběhla; živý placený AI test této změny nebyl proveden.

### 1.10.1 (beta)
- 1.10.1 beta — Oprava ověřování potvrzené série: jednotlivé známky se identifikují přímo bez nadbytečného společného AI dotazu. Neplatná strukturovaná odpověď má nejvýše jedno opakování v povoleném rozpočtu; chyba jedné známky nezastaví ostatní. Když nedoběhne žádná známka série kvůli chybě spojení s AI, souhrn ukáže jednu společnou příčinu. Přesnější diagnostika a čitelnější výpis uložení. Živý placený AI test nebyl proveden. NENÍ oficiální expertíza; GENUINE ground truth = 0.

### 1.10.0 (beta)
- 1.10.0 beta — Rozšířené cenové podklady: nabídky Danner a Schultze, realizace Philea, cílené hledání Michel v Burda a oficiální eBay Browse při dostupném přístupu. Ceny podle stavu, přímé odkazy a popisy; jednotliviny, série a aršíky odděleně. Není potvrzením pravosti ani přesným oceněním fotografie. Placený živý AI test nebyl proveden.

### 1.9.1 (beta)
- 1.9.1 BETA — Dosažený strop útraty za AI se hlásí jako strop, ne jako technická chyba. Dříve ověření při vyčerpaném aplikačním USD stropu psalo „AI identifikace technicky selhala — zkontroluj připojení AI“, ačkoli se žádné volání neodeslalo a nic se nezaplatilo; arch se zastavil uprostřed a opakování okamžitě selhávala. Nově hláška řekne, že byl dosažen strop, dávka se zastaví a rada vede do Klíče & API. USD strop jde nově nastavit, změnit i zrušit přímo v aplikaci (Klíče & API → Strop útraty za placená volání, s potvrzením); dřív jen z kódu. NENÍ oficiální expertíza; kalibrace pravosti neproběhla; živý placený AI test této změny nebyl proveden.

### 1.9.0 (beta)
- 1.9.0 BETA — Podmíněná cenová rozpětí nákupu a prodeje podle stavu, varianty, lepu, jednotky a měny. Nabídky a realizované prodeje jsou oddělené; odhady mají předpoklady a konkrétní zdroje. Výsledky jsou v aplikaci i PDF/DOCX. Citace AI není nezávislé ověření stránky. NENÍ oficiální expertíza; živý placený AI test této změny nebyl proveden.

### 1.8.3 (beta)
- 1.8.3 BETA — Odhad ceny celé dávky včetně úvodního rozpoznání skenu, přehlednější postup přenosu a AI analýz s uplynulým časem. Rychlejší otevření uložených výsledků, pravdivější stručný souhrn, správný čas dokončení a čitelnější PDF/DOCX. Opravy vycházejí z uživatelského testu devíti známek. NENÍ oficiální expertíza; odborná přesnost není kalibrovaná.

### 1.8.2 (beta)
- 1.8.2 BETA — Oprava rozdělení série na tmavém podkladu s bílými okraji skeneru. Před spuštěním série je povinná kontrola a potvrzení výřezů. Neplatná či neúplná odpověď identifikace zastaví navazující analýzy; zpráva, PDF a diagnostika ukazují jednu společnou příčinu. Výřezy zachovávají původní pixely a DPI. NENÍ oficiální expertíza; kalibrace odborné přesnosti neproběhla (validační ground truth = 0).

### 1.8.1 (beta)
- 1.8.1 BETA — Oprava ukládání diagnostických ZIP balíčků v desktopu: povoleno stahování ve WebView2, standardní dialog Uložit jako. Export z obou systémových stránek ověřen ve skutečném desktopovém WebView2; zrušení dialogu nevytvoří soubor. Diagnostický balíček zůstává bez fotografií, promptů, klíčů a sbírkových dat. Nejde o změnu AI analýzy ani oficiální expertízu.

### 1.8.0 (beta)
- 1.8.0 BETA — Zdraví systému, systémová diagnostika a lokální ZIP export bez fotografií, promptů, klíčů a sbírkových dat. Oprava přenosu velkých skenů přes Files API: bloky 1 MiB, obnovení podle potvrzeného offsetu, postup a zrušení mezi bloky bez změny pixelů. NENÍ oficiální expertíza; kalibrace pravosti neproběhla (GENUINE ground truth = 0). Živý placený AI test této změny nebyl proveden.

### 1.7.4 (beta)
- 1.7.4 BETA — oprava přenosu velkých skenů do AI: velké obrázky se nahrávají přes Files API bez zmenšení nebo změny pixelů a během ověření se znovu používají. Zachované lokální kontroly, DPI i originály. Čitelné příčiny selhání přenosu a žádné tvrzení o výsledcích známek, které nebyly identifikovány. NENÍ oficiální expertíza; kalibrace pravosti neproběhla (GENUINE ground truth = 0). Živý placený AI běh této změny nebyl proveden.

### 1.7.3 (beta)
- 1.7.3 BETA — oprava dělení světlých známek na bílém pozadí: části kresby již nejsou další líce. Celý papír líce i rubu včetně bílé nálepky zůstává jedním výřezem. Staré nepotvrzené automatické náhledy se přepočítají; ruční opravy a potvrzené páry se zachovají. Nejasné a oříznuté okraje nejsou falešně vydávány za úplné rozdělení. NENÍ oficiální expertíza; kalibrace pravosti neproběhla (GENUINE ground truth = 0).

### 1.7.2 (beta)
- 1.7.2 BETA — oprava ověření série při nedostupném AI modelu: chyba HTTP 404 se neopakuje a zastaví dávku, nezaměňuje se za špatný výřez či vypnuté kontroly. Podpora aktuálního Gemini 3.5 Flash-Lite s doloženým ceníkem a příprava opakování jedním tlačítkem. Čitelná zpráva série bez technického JSON, zachované analýzy a odkazy; stručný výstup s hlavní příčinou selhání. NENÍ oficiální expertíza.

### 1.7.1 (beta)
- 1.7.1 BETA — při výběru nové známky se ihned odstraní předchozí výsledek, párování, starý rub a údaje předchozí známky. Selhání nahrávání neobnoví starou zprávu. Historie a sbírka zůstávají zachované; výběr kontrol se zachovává. Během ověřování jsou vstupy skenů zamčené. NENÍ oficiální expertíza.

### 1.7.0 (beta)
- Samostatné ceny známek a nezávislé ocenění série/aršíku podle prodejů celku; bez dvojího započtení ve sbírce.
- Kontrola opakovaných instrukcí před ověřením a doporučení dostupného modelu AI.
- Opravené hlášení 600 DPI; stručný i podrobný výstup včetně PDF/DOCX.
- Nepotvrzené zmínky o certifikátech a jasné stavy nedostupných registrů. NENÍ oficiální expertíza.

### 1.6.1 (beta)
- Funkční přepínače čtyř dostupných master promptů přímo u názvu.
- Výběr společný s kontrolami, cenovým odhadem a uloženým ověřením; vypnuté prompty se přeskočí.
- Nepodporované ocenění celé sbírky a kontrola aukčního losu zůstávají neaktivní s vysvětlením. NENÍ oficiální expertíza.

### 1.6.0 (beta)
- Vizuální kontrola a ruční přiřazení líců a rubů před ověřením více známek.
- Úprava výřezů a zachování potvrzené vazby v analýzách, historii, exportech a sbírce.
- Automatické návrhy podle detailů čtyř hran, otočení a zrcadlení; nejisté ruby zůstávají nepřiřazené.
- Automatická přesnost není kalibrovaná; potvrzení uživatelem není potvrzením identity, lepu nebo pravosti. NENÍ oficiální expertíza.

### 1.5.0 (beta)
- Automatické archivování každé analyzované známky, fotografií, výsledků a webových odkazů.
- Ochrana proti duplicitám a obnovení smazaných položek při opakování ověření.
- Hromadné smazání sbírky po potvrzení do vratného koše.
- Delcampe search se kvůli robots nečte; eBay, Delcampe a Apify nejsou zapojené do automatického ověření.
- Uložení neznamená potvrzení pravosti, identity, stavu ani ceny.

### 1.4.0 (beta)
- Automatické posouzení možností snímku, zachování DPI výřezů a místní geometrie každé známky.
- Metadatové odhady zoubkování, orientační centrace, ochrana před nedoloženými závěry AI.
- Katalogové návrhy s konflikty, datované realizace bez duplicit a podmíněný cenový vývoj.
- DPI nejsou kalibrace; katalogy/historie bez dostatečných důkazů nejsou potvrzené; tarif a pojišťovací hodnota zůstávají nezjištěné.

### 1.3.0 (beta)
- Volitelné analýzy a upřesnění pro AI v Jednoduchém ověření.
- Samostatné výsledky jednotlivých známek z listu, kontrola kvality výřezů a společný rozpočet dávky.
- Přesnost dělení reálných aršíků živým Gemini zatím nebyla změřena.

### 1.2.9 (beta)
- Placená volání Gemini se nově zapínají přímo v aplikaci: 🔑 Klíče & API → „Povolit placená volání Gemini“ (zapnutí se potvrzuje, uloží se jen u vás vedle klíče).
- Opraveno: vložený klíč sám nestačil — placený posudek i placené Jednoduché ověření hlásily „nedostupné“, protože povolení šlo dřív nastavit jen v souboru .env.
- Bez zaškrtnutí běží posudek i ověření dál jako neplacená simulace; každé placené spuštění účtuje Google podle ceníku.
- Nemění se: rozsah B (přesné ocenění konkrétní fotografie NENÍ prokázáno), předběžné vizuální posouzení, není oficiální expertíza; kalibrace pravosti neproběhla.

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
