# Rockbox .WPS & .SBS Syntax Highlighting + IntelliSense

This extension adds full development support for Rockbox skin files (`.wps` and `.sbs`) in VS Code / VSCodium.  
It provides syntax highlighting, IntelliSense, hover tooltips, folding regions, and a complete tag reference for all Rockbox skin features.

---

## ✨ Features

### 🎨 Syntax Highlighting
- Highlights all Rockbox skin tags (`%V`, `%xl`, `%pb`, `%?if`, etc.)
- Highlights hex colors (`RRGGBB`)
- Highlights quoted strings
- Dark‑green comments (`# ...`)

### 🧠 IntelliSense (Autocomplete)
- Full snippet library for all Rockbox skin tags (~120)
- Each tag includes:
  - **prefix** (trigger)
  - **syntax**
  - **description**
  - **markdown tooltip**
- Autocomplete triggers automatically when typing `%`

### 💬 Hover Tooltips
Hovering over any tag shows:
- a description of what the tag does  
- syntax  
- usage example  

### 📁 Folding Regions
Supports two region styles:

#### 1) Rockbox‑style sections:

#----------- Main Display -----------#
...
#----------- Main Display -----------#
Kód


#### 2) VS Code‑style regions:

#region Main Display
...
#endregion
Kód


Both styles can be folded and used to organize large WPS/SBS layouts.

### 📄 File Support
- `.wps`
- `.sbs`

---

## 📦 Installation

1. Open VS Code / VSCodium  
2. Press `F1` → **Developer: Install Extension from Location…**  
3. Select the folder containing this extension  
4. Restart the editor  

---

## 🗂 Project Structure

rockbox-wps-sbs-syntax/
├─ syntaxes/
│   └─ rockbox-wps.tmLanguage.json   # Syntax highlighting
├─ snippets/
│   └─ rockbox-wps.json              # All Rockbox tags + tooltips
├─ language-configuration.json        # Comments, folding, brackets
└─ package.json                       # Extension definition
Kód


---

## 🛠 Planned Features
- Outline panel support for sections (Main Display, Status Bar, etc.)
- Color‑coded viewport highlighting
- Syntax validation (linting)
- WPS/SBS template generator

---

## 🤝 Contributing
To add new tags or improve tooltips, edit:

snippets/rockbox-wps.json
Kód


Pull requests and improvements are welcome.

---

## 📜 License
MIT License

---

## 💬 Author
**MiraFicus**  