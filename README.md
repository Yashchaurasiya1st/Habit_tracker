# 🎯 Habit Tracker

A sleek, dark-themed desktop application built with **Electron** to help you build and track daily habits. Visualize your progress with charts, monitor streaks, and stay consistent — all from a beautiful, distraction-free interface.

---

## ✨ Features

- **📊 Dashboard Overview** — See total goals, completed tasks, and remaining items at a glance with stat cards and a donut chart.
- **📈 Daily &amp; Weekly Charts** — Track your daily and weekly completion percentages with interactive Chart.js visualizations.
- **📅 Monthly Habit Grid** — A spreadsheet-style tracker showing every habit x every day of the month, with checkboxes.
- **✏️ Edit Mode** — Add, rename, reorder (drag and drop), and delete habits with an intuitive inline editor.
- **🏆 Top 10 Leaderboard** — See your best-performing habits ranked by completion percentage.
- **🧠 Mental State Tracker** — Log daily mood and motivation scores (1-10) to correlate with your habit performance.
- **↩️ Undo / Redo** — Full undo/redo support so you never lose progress by accident.
- **💾 Auto-Save** — Data is automatically saved to disk (Electron) or localStorage (browser fallback).
- **🌙 Dark Mode** — Premium dark UI with custom CSS variables, glassmorphism accents, and smooth animations.
- **📆 Month/Year Navigation** — Easily switch between months and years to review past performance.

---

## 🖼️ Screenshots

> _Add screenshots of your app here to showcase the UI._
>
> Example:
> ```
> ![Dashboard](screenshots/dashboard.png)
> ![Edit Mode](screenshots/edit-mode.png)
> ```

---

## 🛠️ Tech Stack

| Layer       | Technology                                                   |
| ----------- | ------------------------------------------------------------ |
| Framework   | [Electron](https://www.electronjs.org/) v32+                |
| Frontend    | Vanilla HTML, CSS, JavaScript (single `index.html`)          |
| Charts      | [Chart.js](https://www.chartjs.org/) v4.4.1 (CDN)           |
| Typography  | [Google Fonts](https://fonts.google.com/) — DM Mono + Syne  |
| Build       | [electron-builder](https://www.electron.build/) v24+        |
| Packaging   | Windows Portable (x64)                                      |

---

## 📁 Project Structure

```
Habit_tracker/
├── index.html      # Main UI — HTML + embedded CSS + JavaScript
├── main.js         # Electron main process (window creation + IPC)
├── preload.js      # Context bridge for secure IPC communication
├── package.json    # Dependencies, scripts and build configuration
└── README.md       # This file
```

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v18 or higher
- [npm](https://www.npmjs.com/) (comes with Node.js)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Yashchaurasiya1st/Habit_tracker.git
   cd Habit_tracker
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Run the app:**
   ```bash
   npm start
   ```

### Build for Production

To create a portable Windows executable:

```bash
npm run build
```

The output will be in the `dist/` directory.

---

## 🎮 Usage

1. **Track Habits** — Click the checkboxes in the daily grid to mark habits as done.
2. **Edit Habits** — Click the `Edit` button to enter edit mode where you can:
   - Add new habits
   - Rename existing habits
   - Drag to reorder habits
   - Delete habits
3. **Switch Months** — Use the year and month dropdowns to navigate between different time periods.
4. **Log Mental State** — In the bottom panel, enter daily mood and motivation scores (1-10).
5. **Undo / Redo** — Use the Undo and Redo buttons to revert or reapply changes.
6. **Reset Month** — Click "Reset Month" to clear all data for the current month.

---

## 📦 Data Storage

- **Electron Mode:** Data is saved as `habit_data.json` in the app's user data directory.
- **Browser Mode (fallback):** Data is stored in `localStorage` under the key `habit_tracker_dark_v1`.

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is open source. Consider adding a [LICENSE](https://choosealicense.com/) file to specify how others can use your code.

---

## 👤 Author

**Yash Chaurasiya** — [@Yashchaurasiya1st](https://github.com/Yashchaurasiya1st)

---

<p align="center">
  Made with ❤️ for building better habits
</p>

