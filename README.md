# Slovíčka 🎈 (WordLang)

Jednoduchá, hravá webová hra pro děti na výslovnost slovíček. Zobrazí české slovo
velkými písmeny a po stisku tlačítka s vlajkou ho přečte nahlas v cílovém jazyce
(angličtina 🇺🇸, němčina 🇩🇪, španělština 🇪🇸).

**Živá verze:** https://mlutonsky.github.io/wordlang/

## Jak to funguje

- `index.html` – celá aplikace (HTML + CSS + JS v jednom souboru, bez závislostí).
- `words.csv` – slovník v UTF-8. Čtení nahlas zajišťuje vestavěná syntéza řeči
  prohlížeče (Web Speech API), takže není potřeba žádný klíč ani server navíc.

## Ovládání

- **Emoji / české slovo** – ťuknutím se slovo přečte nahlas v češtině 🇨🇿.
- **Tlačítka jazyků** – přečtou slovo nahlas.
- **◀ / ▶** – předchozí / další slovo.
- **🎲** – náhodné slovo.
- Na PC fungují i šipky (◀ ▶), mezerník (náhodně), klávesa 0 (čeština) a klávesy 1–3 (jazyky).

## Přidání slovíček

Stačí upravit `words.csv` – jeden řádek = jedno slovo:

```
cs,en,de,es,emoji
PES,dog,Hund,perro,🐶
```

Sloupec `emoji` je nepovinný. Po úpravě nahraj soubor zpět do repozitáře.

## Poznámka k hlasům

Kvalita a dostupnost hlasů závisí na zařízení/prohlížeči. Pokud nějaký jazyk na
daném zařízení nemá nainstalovaný hlas, je možné ho doinstalovat v nastavení
systému (sekce převod textu na řeč / hlasy).
