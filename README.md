## 💻 Task Juggler and Thumbnails Slider

A lightweight Windows utility for power users who juggle many folders, files, and windows at once. It combines a customizable quick-access **launcher** with a **thumbnails slider** for fast visual browsing, plus built-in virtual desktop switching.

## ⭐ What it does

- **Launcher** — A compact, themeable panel for jumping between your favorite folders, switching active windows/tabs, and managing exceptions, all from one hotkey-triggered popup.
- **Thumbnails Slider** — Resize and preview thumbnails on the fly, in multiple slider sizes, so you can scan through images or files without opening each one.
- **Selection Tools** — Select files by pattern, select all items of the same extension, and keep a history of your selections so you can restore or backtrack to a previous selection instantly.
- **Virtual Desktop Integration** — Add, remove, and cycle through virtual desktops directly from the launcher, with visual indicators for the active desktop.
- **Fully Themeable** — Pick colors for the header, background, progress indicators, and more, with a built-in color picker and several ready-made themes.

## 📌 How to Use

1. Download and extract **`AIO_Task_Juggler_and_Thumbnails_Slider_26_08_12_V1.1.7.6.zip`** — this all-in-one package contains everything needed, already extracted and ready to run.
2. Launch only the **main executable** (`Task_Juggler_and_Thumbnails_Slider_26_08_12_V1.1.7.6_X64.exe`).
3. Do **not** run `VD_DATA.exe` directly — it's a background helper module used internally for virtual desktop detection and is launched automatically by the main app when needed.

## 🌞 Launcher Themes

<table>
<tr>
<td align="center"><b>Midnight Blue</b><br><img src="Images/A1.png" width="220"></td>
<td align="center"><b>Dark Red</b><br><img src="Images/A2.png" width="220"></td>
</tr>
<tr>
<td align="center"><b>Dark Green</b><br><img src="Images/A3.png" width="220"></td>
<td align="center"><b>Midnight Purple</b><br><img src="Images/A4.png" width="220"></td>
</tr>
</table>

Four ready-made color themes for the launcher, switchable at any time from the settings panel.

**♦️Visual overview:**


![Launcher Overview](Images/A5.png)


*Breakdown of the launcher's main visual elements and layout.*

## 🔧Settings

<table>
<tr>
<td align="center"><b>Favorite Folders</b><br><img src="Images/B1.png" width="200"><br><sub>Manage the folders that appear in your launcher for quick access.</sub></td>
<td align="center"><b>Switcher</b><br><img src="Images/B2.png" width="200"><br><sub>Configure how window/tab switching behaves.</sub></td>
<td align="center"><b>Exceptions</b><br><img src="Images/B3.png" width="200"><br><sub>Exclude specific folders or apps from launcher actions.</sub></td>
</tr>
<tr>
<td align="center"><b>Theme</b><br><img src="Images/B4.png" width="200"><br><sub>Customize colors and appearance of the launcher.</sub></td>
<td align="center"><b>Extra</b><br><img src="Images/B5.png" width="200"><br><sub>Additional options and fine-tuning settings.</sub></td>
<td align="center"><b>Color Picker</b><br><img src="Images/B6.png" width="200"><br><sub>Built-in color picker for custom theme colors.</sub></td>
</tr>
</table>

## 🔵 Thumbnails Slider

<table>
<tr>
<td align="center"><b>Slider Settings</b><br><img src="Images/C1.png" width="220"><br><sub>Configure slider behavior and appearance.</sub></td>
<td align="center"><b>Slider Sizes</b><br><img src="Images/C2.png" width="220"><br><sub>Choose between multiple slider sizes to fit your workflow.</sub></td>
</tr>
<tr>
<td align="center"><b>Pattern Selection</b><br><img src="Images/C3.png" width="220"><br><sub>Select files by pattern using a dedicated input dialog.</sub></td>
<td align="center"><b>Selection History</b><br><img src="Images/C4.png" width="220"><br><sub>Browse and restore previous selections.</sub></td>
</tr>
</table>

# 🎥 Demos 👇

<table>
<tr>
<td align="center">
<b>Resize Preview</b><br>
<img src="Gif/E1.gif" width="320"><br>
<sub>Live preview while resizing the thumbnails slider.</sub>
</td>
<td align="center">
<b>Lister (Opus) Tab Switch + Virtual Desktop</b><br>
<img src="Gif/E2.gif" width="320"><br>
<sub>Switching between Opus lister tabs alongside virtual desktops.</sub>
</td>
</tr>
<tr>
<td align="center">
<b>Minimize / Restore / Cycle Listers</b><br>
<img src="Gif/E3.gif" width="320"><br>
<sub>Minimize, restore, and cycle through all open Opus listers.</sub>
</td>
<td align="center">
<b>App Switch + Explorer Switch</b><br>
<img src="Gif/E4.gif" width="320"><br>
<sub>Quickly switch between running apps and Explorer windows.</sub>
</td>
</tr>
<tr>
<td align="center">
<b>Slider in Action</b><br>
<img src="Gif/E5.gif" width="320"><br>
<sub>The thumbnails slider being used to browse files visually.</sub>
</td>
<td align="center">
<b>Pattern Select + Backtrack + History</b><br>
<img src="Gif/E6.gif" width="320"><br>
<sub>Selecting by pattern, restoring a backtrack, and using the history GUI.</sub>
</td>
</tr>
</table>

**Help Reference:**



![Help](Gif/E7.gif)


*How to access the built-in help panel.*
___
## ✔️ Icons

All icons shown in the demos and screenshots are included in **`ICO.zip`**. They are not applied automatically — after extracting the archive, you'll need to manually assign each icon to its corresponding entry (favorite folder, app, folder type, etc.) from the Settings panel to match the look shown in this repo.

## ♥️ Favorite Folders — Syntax

Favorite folders are listed one per line in the **Favorites Folders** tab. Each line supports an optional custom name and display modifiers.

```
PATH
PATH|Custom Name
PATH|Custom Name/B
PATH|Custom Name/HEXCOLOR
//PATH|Disabled Entry
```

- `PATH` — the folder path (required)
- `|Custom Name` — optional display name instead of the raw path
- `/B` — makes the entry bold
- `/HEXCOLOR` — sets a custom text color (e.g. `/FF6B6B`), can be combined with `/B` in any order
- `//` at the start of a line disables/hides that entry without deleting it

**👇Examples:**
```

C:\Projects
C:\Users\Me\Documents|My Documents
D:\Media|Media Library/FF6B6B
C:\Work\Reports|Reports/B
//C:\Archive|Old Archive (temporarily disabled)
```

## 🔗 Pattern Selection — Syntax

The pattern selector (opened from the pattern dialog) supports several matching modes, entered as a single string.

| Syntax | Behavior |
|---|---|
| `ext1,ext2,ext3` | Select all files matching these extensions |
| `/name` | Select items whose name contains "name" |
| `/^name` | Select items whose name **starts with** "name" |
| `/name$` | Select items whose name **ends with** "name" |
| `/name1/name2` | Select items matching **any** of multiple names |
| `/name:ext1,ext2` or `name:ext1,ext2` | Select items matching a name **and** extension filter |
| `re:pattern` | Select items using a full regex pattern |
| `/F` (appended flag) | Include folders in the results |

**👇Examples:**
```

avi,mp4,mkv          → all video files
/report              → items containing "report"
/^intro               → items starting with "intro"
/outro$               → items ending with "outro"
/movie/show:mp4,mkv   → "movie" or "show" items with mp4/mkv extension
re:^\d{4}-\d{2}-\d{2} → regex match (e.g. date-prefixed files)
avi,mp4/F             → video files, folders included
```

## 🎨 Active Tab Indicator & Indentation

Found under **Settings → Extra tab**. This controls how the currently active Lister tab is visually marked in the launcher list.

- **Indicator** — the symbol shown next to the active tab (default: `▶`)
- **Indent** — how many spaces to add before the indicator, from 0 to 20

The same principle applies to the **Virtual Desktop indicator**, configured in the VD section: a symbol (default: `◆`) with its own adjustable indent, used to mark the currently active desktop in the list.

## 🖥️🖥️ Virtual Desktop Switching & Auto-Jump

Each virtual desktop appears as its own entry in the launcher, letting you switch desktops with a single click. You can also add or remove virtual desktops directly from the same panel.

When **Quick Jump** is enabled (Settings), clicking a folder, app, or Lister tab that lives on a different virtual desktop will automatically switch you to the correct desktop before activating that window — no manual desktop switching needed.

## ➕ Status Bar

The status bar at the bottom of the launcher gives a live summary of what's currently listed:

- **FAV** — number of favorite folders
- **EXP** — number of open Explorer windows
- **APP** — number of tracked running apps
- **TAB** — number of Opus Lister tabs
- **LIS** — number of open Listers

Items with a virtual desktop location also show a short desktop tag (e.g. `D1`, `D2`) at the right edge, indicating which virtual desktop that item currently lives on.

## ✔️ Enable Only What You Need

Every major feature — favorite folders, Explorer window listing, app listing, Opus tab listing, status bar, virtual desktop switching, and more — has its own checkbox in the Settings panel. Nothing is forced on: disable the modules you don't use and keep only the features that fit your workflow.
```
___

## 🎯 Quick Jump vs. Reactivate Mode

Found in **Settings**, this toggle controls how the launcher handles items that are already open.

- **🖍️Quick Jump enabled** — clicking a folder, app, or Opus tab that's already open reuses the existing window: it switches to the correct virtual desktop (if needed) and simply brings that window to the front, without opening anything new.
- **🖊️Quick Jump disabled** — instead of just focusing the window, the launcher fully reactivates it: for Opus tabs it switches to the correct tab inside the Lister, for apps and Explorer windows it restores/reactivates the window before bringing it forward.

In short: Quick Jump is the faster "just show it" mode, while disabling it forces a full reactivate + tab/window switch every time.

## 📂 Default File Manager

The **"Use Current File Manager"** option (Settings → Favorites Folders tab) determines which file manager opens your favorite folders — your current default Explorer replacement (e.g. Explorer itself, Directory Opus, or any other file manager set as default on your system) instead of forcing a specific one.

## ✏️ Custom Virtual Desktop Name

In the **Extra** section of the settings, you can enable **Use Custom Name** and set your own label for virtual desktops instead of the default "Desktop 1, Desktop 2...". For example, setting the name to `Desk` will display desktops as `Desk 1`, `Desk 2`, `Desk 3`, etc.

## 📚 Header Colors

Each category header in the launcher list has its own configurable color, set individually in the Theme tab:

- Favorite Folders header color
- Explorer Windows header color
- Application Switcher header color
- Opus Tabs header color
- Virtual Desktop header color

## 🔗 Active Item Color & Bold

Each item type can independently show the currently active entry in bold and/or a custom color:

- **Opus Tab** — bold toggle + color for the active tab path
- **Explorer** — bold toggle + color for the active Explorer window path
- **Favorite Folder** — bold toggle + color for the active folder
- **Application** — bold toggle + color for the active app
- **Virtual Desktop** — bold toggle + color for the currently active desktop

## ⛏️ Virtual Desktop Add / Remove Icons

The icons used for the **Add Virtual Desktop** and **Remove Virtual Desktop** buttons can each be set to a custom icon path in the VD settings, letting you replace the default system icons with your own.

## 📌 Minimized State Indicators

- **Explorer windows & Apps** — a minimized item is marked with a 🔻 symbol before its name. No bold and no custom color are applied to this marker; it stays plain to keep it visually distinct from active/highlighted entries.
- **Opus Listers** — when a Lister is minimized, its header (e.g. `Lister 1`) is prefixed with the same 🔻 symbol, but unlike Explorer/App entries it's always rendered in **white and bold**, so minimized Listers stand out clearly at a glance.

___


## 🔥 Downloads

- `Task_Juggler_and_Thumbnails_Slider_26_08_12_V1.1.7.6_X64.exe` — standalone executable
- `Task_Juggler_and_Thumbnails_Slider_26_08_12_V1.1.7.6_X64.zip` — portable version
- `AIO_Task_Juggler_and_Thumbnails_Slider_26_08_12_V1.1.7.6.zip` — all-in-one package (extract and run, includes everything)
- `ICO.zip` — icon pack
- `VD_DATA.exe` / `VD_DATA.zip` — internal virtual desktop helper (not meant to be run manually)

---
Copyright © AndrianAngel ❤️ — All rights reserved.
