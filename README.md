# 🎯 Habit Tracker

> A dark-themed desktop app built with Electron to track daily habits, visualize weekly progress, and stay consistent — month after month.

![Platform](https://img.shields.io/badge/platform-Windows-blue?style=flat-square&logo=windows)
![Electron](https://img.shields.io/badge/Electron-32.x-47848F?style=flat-square&logo=electron)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![Status](https://img.shields.io/badge/status-active-brightgreen?style=flat-square)

---

## 📸 Preview

> **Dashboard** — Monthly grid, progress charts, stats overview and mental state tracker all in one dark interface.

*(Add a screenshot here: drag an image into the repo on GitHub and paste the link)*

---

## ✨ Features

| Feature | Description |
|---|---|
| 📅 Monthly Habit Grid | Checkbox for every habit × every day of the month |
| 📊 Daily & Weekly Charts | Bar charts showing completion % over time |
| 🍩 Overall Stats Donut | Visual breakdown of completed vs remaining |
| ✏️ Edit Mode | Add, rename, reorder (drag & drop), and delete habits in one panel |
| 🏆 Top 10 Leaderboard | Habits ranked by completion percentage |
| 🧠 Mental State Tracker | Log daily mood and motivation (1–10 scale) |
| ↩️ Undo / Redo | Up to 80-step history — never lose progress by accident |
| 💾 Auto-Save | Saves to disk on every action — no save button needed |
| 📆 Month Navigation | Switch between any month/year to review past data |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Framework | [Electron](https://www.electronjs.org/) v32 |
| Frontend | Vanilla HTML + CSS + JavaScript (`index.html`) |
| Charts | [Chart.js](https://www.chartjs.org/) v4.4.1 |
| Fonts | Google Fonts — DM Mono + Syne |
| Build Tool | [electron-builder](https://www.electron.build/) v24 |
| Storage | File system via IPC (`habit_data.json`) |
| Output | Windows Portable EXE (x64) |

---

## 📁 Project Structure

```
Habit_tracker/
├── index.html       # Full app UI — HTML, CSS, and JS in one file
├── main.js          # Electron main process — window + IPC handlers
├── preload.js       # Secure context bridge for renderer ↔ main IPC
├── package.json     # Scripts, build config, and dependencies
└── README.md        # You are here
```

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v18 or higher (LTS recommended)
- npm (comes with Node.js)
- Windows 10/11 (for building the `.exe`)

### Run in Development

```bash
# 1. Clone the repo
git clone https://github.com/Yashchaurasiya1st/Habit_tracker.git
cd Habit_tracker

# 2. Install dependencies
npm install

# 3. Launch the app
npm start
```

### Build Windows EXE

> ⚠️ Run Command Prompt **as Administrator** to avoid symlink permission errors on Windows.

```bash
npm run build
```

Output: `dist/Habit Tracker 1.0.0.exe` — portable, no installation needed.

---

## 🎮 How to Use

1. **Check habits** — Click any checkbox in the grid to mark a habit done for that day
2. **Edit mode** — Click **✏ Edit** to:
   - Add a new habit (type name → press Enter or click **+ Add Habit**)
   - Rename a habit (click the name field and type)
   - Reorder habits (drag the ☰ handle or use ▲▼ buttons)
   - Delete a habit (click ✕)
   - Click **✕ Done Editing** to close and auto-save all changes
3. **Switch months** — Use the year and month dropdowns at the top
4. **Mental state** — Enter mood and motivation scores (1–10) in the bottom panel
5. **Undo / Redo** — Use ↩ and ↪ buttons to step through your change history
6. **Reset Month** — Clears all checkboxes for the current month (asks for confirmation)

---

## 💾 Data Storage

| Mode | Location |
|---|---|
| Electron (`.exe`) | `%APPDATA%\habit-tracker\habit_data.json` |
| Browser (fallback) | `localStorage` → key: `habit_tracker_dark_v1` |

Data is saved automatically on every action — no manual save required.

---

## 📦 Download

Head to the [Releases](https://github.com/Yashchaurasiya1st/Habit_tracker/releases) page to download the latest portable `.exe` for Windows.

No installation required — just download and double-click to run.

---

## ⚠️ Things to Fix / Add

- [ ] Add a screenshot to the Preview section above
- [ ] Add a `.gitignore` file to exclude `node_modules/` and `dist/`
- [ ] Add a `LICENSE` file (MIT recommended)
- [ ] Add repo description and topics on GitHub sidebar (e.g. `electron`, `habit-tracker`, `dark-theme`, `productivity`)

---

## 🤝 Contributing

1. Fork this repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

This project is open source. Consider adding a [LICENSE](https://choosealicense.com/licenses/mit/) file to let others freely use and build on this project.

---

## 👤 Author

**Yash Chaurasiya**
- GitHub: [@Yashchaurasiya1st](https://github.com/Yashchaurasiya1st)
- Project: [Habit_tracker](https://github.com/Yashchaurasiya1st/Habit_tracker)

---

*Built with ❤️ to make consistency a daily habit.*
