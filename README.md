
# CAP'2ER – Větvení dotazníku podle typu výroby

Tento repozitář obsahuje strukturu otázek z dotazníku CAP'2ER, rozdělenou podle typu výroby – mléčná nebo masná.

## 📁 Soubory

- `CAP2ER_Otazky_Dle_Vyroby.json` – Hlavní JSON soubor obsahující mapu sekcí a otázek pro jednotlivé typy výroby.
- `CAP2ER_Otazky_Dle_Vyroby.html` – HTML náhled pro čitelné zobrazení dat v prohlížeči.

## 🧭 Použití

- Pro načtení JSON struktury v aplikaci:
  ```js
  fetch('CAP2ER_Otazky_Dle_Vyroby.json')
    .then(res => res.json())
    .then(data => console.log(data));
  ```

- Každý typ výroby (`Mléčná výroba`, `Masná výroba`) obsahuje seznam sekcí, které dále obsahují pole s kódem otázky a textem otázky.

## 🔍 Příklad JSON struktury

```json
{
  "Mléčná výroba": {
    "Stáda": [
      {
        "kod": "TROUP_RACE1_BL",
        "otazka": "Mléčné plemeno"
      },
      ...
    ],
    ...
  },
  ...
}
```

## 📌 Licence

Projekt je otevřený pro potřeby implementace CAP'2ER dotazníku. Vznikl v rámci podpory projektu OK CARBON.
