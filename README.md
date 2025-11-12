# APBingo Web

This repository contains the **APBingo** webpage implementation.  
It is designed to send checks to the Archipelago server and has been updated for **archipelago.js v2.0.4**.

---

## 🎯 Usage

### 1. Running the Bingo Board
- Unzip the patch and open the `APBingoWeb.html` file in your browser.
- The board will attempt to load configuration automatically.  
  - You can provide configuration via **URL parameters** or by editing the HTML directly.

### 2. Configuration Options

#### ✅ URL Parameters (recommended for OBS or to avoid prompts)
You can pass server configuration directly in the URL:

```
APBingoWeb.html?server=archipelago.gg:38281&username=Player1&password=
```

- `server` → Archipelago server address and port (e.g., `archipelago.gg:60355`)
- `username` → Your chosen player name
- `password` → Leave empty if no password is required

This method is especially useful when embedding the page in **OBS** or when you want to skip interactive prompts.

---

#### ✅ Editing the HTML File
Alternatively, you can hardcode your configuration inside the HTML file:

```html
<script type="module">
  let server   = undefined;   // Line 40
  let password = undefined;   // Line 41
  let username = undefined;   // Line 42
</script>
```

Replace the `undefined` values with your desired settings.  
For example:

```html
<script type="module">
  let server   = "archipelago.gg:38281";
  let password = "";
  let username = "Player1";
</script>
```


## 📦 Repository Location
The main repository has been moved from GitHub to:

👉 [https://git.moyskleytech.com/ObsidianMakerDevelopment/APBingoWeb-OBS](https://git.moyskleytech.com/ObsidianMakerDevelopment/APBingoWeb-OBS)

