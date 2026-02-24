# Rockbox .WPS & .SBS Syntax Highlighting + IntelliSense

Rozšíření pro VS Code / VSCodium, které přidává kompletní podporu pro tvorbu Rockbox skinů (`.wps` a `.sbs`).  
Cílem je zpříjemnit a zrychlit práci na skinech díky zvýraznění syntaxe, našeptávání, tooltipům a přehledným sekcím.

---

## ✨ Funkce

### 🎨 Syntax Highlighting
- zvýraznění všech Rockbox tagů (`%V`, `%xl`, `%pb`, `%?if`, …)
- zvýraznění hex barev (`RRGGBB`)
- zvýraznění textů v uvozovkách
- tmavě zelené komentáře (`# ...`)

### 🧠 IntelliSense (Autocomplete)
- kompletní sada snippetů pro všechny Rockbox tagy (~120)
- každý tag má:
  - **prefix** (spouštěč)
  - **syntax**
  - **popis**
  - **markdown tooltip** (zobrazený při najetí myší)
- našeptávání funguje při psaní `%`

### 💬 Hover Tooltipy
- při najetí myší na tag se zobrazí:
  - popis funkce
  - syntaxe
  - příklad použití

### 📁 Folding Regions
Podpora dvou stylů sekcí:

#### 1) Rockbox styl:

#----------- Main Display -----------#
...
#----------- Main Display -----------#



#### 2) VS Code styl:

#region Main Display
...
#endregion



Obě varianty lze sbalit a přehledně organizovat.

### 📄 Podpora souborů
- `.wps`
- `.sbs`

---

## 📦 Instalace

1. Otevři VS Code / VSCodium  
2. `F1` → **Developer: Install Extension from Location…**  
3. Vyber složku s tímto rozšířením  
4. Restartuj editor

---

## 🗂 Struktura projektu

rockbox-wps-sbs-syntax/
├─ syntaxes/
│   └─ rockbox-wps.tmLanguage.json   # zvýraznění syntaxe
├─ snippets/
│   └─ rockbox-wps.json              # všechny Rockbox tagy + tooltipy
├─ language-configuration.json        # komentáře, folding, brackets
└─ package.json                       # definice rozšíření



---

## 🛠 Plánované funkce
- outline panel pro sekce (`Main Display`, `Status Bar`, …)
- zvýraznění viewportů různými barvami
- validátor syntaxe (linting)
- generátor šablon pro WPS/SBS

---

## 🤝 Přispívání
Pokud chceš přidat nové tagy, vylepšit tooltipy nebo rozšířit funkcionalitu, uprav soubor:

snippets/rockbox-wps.json



---

## 📜 Licence
MIT License

---

## 💬 Autor
**MiraFicus**  