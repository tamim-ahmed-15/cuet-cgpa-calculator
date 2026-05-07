<h1 align="center">CUET CGPA Calculator</h1>

<p align="center">
  <strong>A Chrome extension that automatically calculates your GPA &amp; CGPA from the CUET Student Portal.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/manifest-v3-blue?style=flat-square" alt="Manifest V3">
  <img src="https://img.shields.io/badge/license-MIT-green?style=flat-square" alt="MIT License">
  <img src="https://img.shields.io/badge/platform-Chrome-yellow?style=flat-square&logo=googlechrome&logoColor=white" alt="Chrome">
  <img src="https://img.shields.io/badge/university-CUET-purple?style=flat-square" alt="CUET">
</p>

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 📊 **Semester GPA** | Calculates GPA for each Level-Term automatically |
| 🎓 **Overall CGPA** | Computes cumulative CGPA across all semesters |
| 🎯 **Target CGPA Planner** | Set a target CGPA and find out the GPA you need in remaining semesters |
| 📈 **Performance Graph** | Visual line chart showing your GPA trend over semesters |
| 🔒 **Privacy First** | All calculations happen locally — no data leaves your browser |
| 🌙 **Premium Dark UI** | Glassmorphism design with smooth animations |

---

## 📸 How It Works

1. Log in to **[course.cuet.ac.bd](https://course.cuet.ac.bd)**
2. Navigate to the **Published Result** page
3. Click the **purple floating button** (bottom-right corner)
4. Your semester-wise GPA, overall CGPA, and performance graph appear instantly!

---

## 🚀 Installation

### Step 1 — Download

Download the latest release as a ZIP file and extract it, or clone the repo:

```bash
git clone https://github.com/YOUR_USERNAME/cuet-cgpa-calculator.git
```

### Step 2 — Load in Chrome

1. Open Chrome and go to `chrome://extensions/`
2. Enable **Developer mode** (toggle in the top-right corner)
3. Click **"Load unpacked"**
4. Select the `cuet-cgpa-calculator` folder
5. Done! ✅ The extension icon appears in your toolbar

---

## 🧮 Grade Point Scale

The extension uses the standard CUET / Bangladesh grading scale:

| Grade | Point | Grade | Point |
|-------|-------|-------|-------|
| A+    | 4.00  | C+    | 2.50  |
| A     | 3.75  | C     | 2.25  |
| A-    | 3.50  | D     | 2.00  |
| B+    | 3.25  | F     | 0.00  |
| B     | 3.00  |       |       |
| B-    | 2.75  |       |       |

### Formulas

- **GPA** = `Σ(credit × grade_point) / Σ(credit)` — per semester
- **CGPA** = `Σ(all credits × grade_point) / Σ(all credits)` — cumulative
- **Required GPA** = `(target × total_credits - earned_points) / remaining_credits`

---

## 🗂️ Project Structure

```
cuet-cgpa-calculator/
├── manifest.json       # Chrome Extension manifest (V3)
├── content.js          # Main logic — reads results, computes GPA/CGPA, renders UI
├── content.css         # Dark glassmorphism panel styles
├── popup.html          # Extension popup with usage instructions
├── README.md
└── icons/
    ├── icon48.png      # Toolbar icon
    └── icon128.png     # Store / settings icon
```

---

## 🎯 Three Tabs

### 📋 Results Tab
- Lists every semester (Level-Term) with its GPA
- Click any semester card to expand and see individual course grades
- Color-coded GPA: 🟢 Excellent (≥3.5) · 🔵 Good (≥3.0) · 🟡 Average (≥2.5) · 🔴 Low (<2.5)

### 🎯 Target Tab
- Enter your **target CGPA** (saved for next time)
- Enter your **remaining credits**
- Get the exact GPA you need with a difficulty rating:
  - ✅ Achievable · 💪 Challenging · 🔥 Very Hard · ❌ Impossible

### 📈 Graph Tab
- Line chart showing your GPA trend across semesters
- Gradient area fill under the curve
- Dashed CGPA reference line
- GPA values displayed above each data point

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve the extension:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE) — feel free to use, modify, and distribute.

---

## 🙋 FAQ

**Q: Does this extension collect my data?**
> No. Everything runs locally in your browser. No data is sent to any server.

**Q: Why isn't the floating button appearing?**
> Make sure you are on the Published Result page after logging in. The extension activates only on `course.cuet.ac.bd` pages.

**Q: Will it work on Firefox / Edge?**
> Currently built for Chrome. Edge (Chromium-based) should work with the same installation steps. Firefox would require minor modifications.

---

<p align="center">
  Made with ❤️ for CUET Students
</p>
