# Aplikace ke stažení

Veřejné stažení instalátorů mých aplikací pro Windows. Instalátory jsou **zaheslované** —
stáhneš `-Setup.exe`, spustíš, zadáš heslo a nainstaluješ. Aplikace se pak při spuštění samy
nabízí k aktualizaci.

## Aplikace

- **BudLine Panel** — zpracování turnusů a kontrola mzdy / výplatních pásek pro řidiče.
- **Meal Planner** — plánovač jídel, lednice, nákupní seznam a recepty.
- **Italia Travel Planner** — plánovač cesty po Itálii (itinerář, mapa, roadtrip, rozpočet).
- **Collection** — evidence sbírky (numismatika / filatelie) s rozpoznáváním přes AI.

## Stažení

| Aplikace | Verze | Instalátor |
|---|---|---|
| BudLine Panel | 1.2.3 | [BudLinePanel-v1.2.3-Setup.exe](https://github.com/bludek69-lgtm/aplikace/releases/download/apps/BudLinePanel-v1.2.3-Setup.exe) |
| Meal Planner | 0.8.4 | [MealPlanner-v0.8.4-Setup.exe](https://github.com/bludek69-lgtm/aplikace/releases/download/apps/MealPlanner-v0.8.4-Setup.exe) |
| Italia Travel Planner | 0.7.4 | [ItaliaTravel-v0.7.4-Setup.exe](https://github.com/bludek69-lgtm/aplikace/releases/download/apps/ItaliaTravel-v0.7.4-Setup.exe) |
| Collection | 1.1.3 | [Collection-v1.1.3-Setup.exe](https://github.com/bludek69-lgtm/aplikace/releases/download/apps/Collection-v1.1.3-Setup.exe) |

Aktuální verze a kontrolní součty jsou vždy v [`latest.json`](https://github.com/bludek69-lgtm/aplikace/blob/main/latest.json)
a v [`CHECKSUMS.txt`](https://github.com/bludek69-lgtm/aplikace/blob/main/CHECKSUMS.txt).
Přehled změn najdeš v [`CHANGELOG.md`](https://github.com/bludek69-lgtm/aplikace/blob/main/CHANGELOG.md).

## Heslo k instalaci

Instalátory jsou zaheslované. **Heslo neposílám přes GitHub** — dostaneš ho ode mě zvlášť
(SMS / Signal). Každá aplikace má vlastní heslo. Samotný stažený `.exe` je bez hesla
nepoužitelný.

## Instalace krok za krokem

1. Klikni na odkaz výše → stáhne se `-Setup.exe`.
2. Spusť stažený soubor.
3. Windows může ukázat **„Windows ochránil váš počítač" (SmartScreen)** — je to jen proto,
   že instalátor nemá placený podpis. Klikni **„Další informace" → „Přesto spustit"**.
4. Zadej **heslo**, které jsem ti poslal zvlášť.
5. Nech výchozí složku a doklikej „Další / Dokončit".
6. Hotovo — aplikaci spustíš ze zástupce na ploše / v nabídce Start.

## Aktualizace

Když vyjde novější verze, aplikace ti ji při spuštění sama nabídne a po potvrzení se
aktualizuje. Pokud tichá aktualizace nemá k dispozici heslo, nabídne ručního průvodce —
není to chyba.

## Ověření staženého souboru (volitelné)

V PowerShellu spočítej kontrolní součet a porovnej s `CHECKSUMS.txt`:

```powershell
Get-FileHash -Algorithm SHA256 .\BudLinePanel-v1.2.3-Setup.exe
```
