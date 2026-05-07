<h1 align="center">CUET CGPA Calculator</h1>

<p align="center">
	<strong>A Chrome/Chromium extension that automatically calculates your GPA and CGPA from the CUET result page.</strong>
</p>

<p align="center">
	<img src="https://img.shields.io/badge/manifest-v3-blue?style=flat-square" alt="Manifest V3">
	<img src="https://img.shields.io/badge/platform-Chrome%20%7C%20Chromium-yellow?style=flat-square&logo=googlechrome&logoColor=white" alt="Chrome and Chromium">
	<img src="https://img.shields.io/badge/university-CUET-purple?style=flat-square" alt="CUET">
</p>

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 📊 **Semester GPA** | Calculates GPA for each Level-Term automatically |
| 🎓 **Overall CGPA** | Computes cumulative CGPA across all semesters |
| 🎯 **Target CGPA Planner** | Set a target CGPA and estimate the GPA needed in remaining credits |
| 📈 **Performance Graph** | Visual line chart showing your GPA trend over semesters |
| 🔒 **Privacy First** | All calculations happen locally in your browser |
| 🌙 **Premium Dark UI** | Glassmorphism-inspired panel with smooth animations |

---

## 📸 How It Works

1. Log in to **[course.cuet.ac.bd](https://course.cuet.ac.bd)**
2. Navigate to the **Published Result** page
3. Click the **purple floating button** at the bottom-right corner
4. View your semester-wise GPA, overall CGPA, target GPA planner, and performance graph instantly

---

## 🚀 Installation

### Step 1 — Download

Download the repository as a ZIP file from GitHub and extract it, or clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/cuet-cgpa-calculator.git
```

### Step 2 — Load in Chrome

1. Open Chrome or another Chromium-based browser and go to `chrome://extensions/`
2. Enable **Developer mode** in the top-right corner
3. Click **Load unpacked**
4. Select the extracted `cuet-cgpa-calculator` folder
5. The extension icon should now appear in your toolbar

### If You Download the ZIP From GitHub

1. Download the repository as a ZIP file from GitHub
2. Extract the ZIP to a normal folder on your computer
3. Open `chrome://extensions/` and enable **Developer mode**
4. Click **Load unpacked**
5. Select the extracted project folder, not the ZIP file itself

Chrome extensions cannot be loaded directly from a compressed ZIP file, so the folder must be extracted first.

---

## 🧮 Grade Point Scale

The extension uses the CUET / Bangladesh grading scale:

| Grade | Point | Grade | Point |
|-------|-------|-------|-------|
| A+    | 4.00  | C+    | 2.50  |
| A     | 3.75  | C     | 2.25  |
| A-    | 3.50  | D     | 2.00  |
| B+    | 3.25  | F     | 0.00  |
| B     | 3.00  |       |       |
| B-    | 2.75  |       |       |

### Formulas

- **GPA** = $\Sigma(credit \times grade\_point) / \Sigma(credit)$ per semester
- **CGPA** = $\Sigma(all\ credits \times grade\_point) / \Sigma(all\ credits)$ across all semesters
- **Required GPA** = $(target \times total\_credits - earned\_points) / remaining\_credits$

---

## 🗂️ Project Structure

```
cuet-cgpa-calculator/
├── manifest.json       # Chrome extension manifest (Manifest V3)
├── content.js          # Main logic: reads results, computes GPA/CGPA, renders the panel
├── content.css         # Styles for the floating button and calculator UI
├── popup.html          # Extension popup with usage instructions
├── README.md
└── icons/
		├── icon48.png      # Toolbar icon
		├── icon128.png     # Larger extension icon
		├── generate_icons.html
		└── generate.ps1    # Local icon-generation helper
```

---

## 🎯 Main Tabs

### 📋 Results Tab
- Lists each semester (Level-Term) with its GPA
- Click any semester card to expand and view individual course grades
- GPA colors help you scan performance quickly

### 🎯 Target Tab
- Enter your target CGPA
- Enter your remaining credits
- Get the GPA you need to reach your goal
- The target value is saved locally for next time

### 📈 Graph Tab
- Line chart showing your GPA trend across semesters
- Gradient area fill under the curve
- Dashed CGPA reference line
- GPA values displayed above each point

---

## 🔒 Privacy

This extension processes the CUET result page locally in your browser. It does not send your result data to a server.

---

## 🌐 Browser Support

This project is designed for Chrome and other Chromium-based browsers that support Manifest V3 extensions.

---

## 🙋 FAQ

**Q: Does this extension collect my data?**  
> No. Everything runs locally in your browser.

**Q: Why isn't the floating button appearing?**  
> Make sure you are on the Published Result page after logging in. The extension activates only on `course.cuet.ac.bd` pages.

**Q: Will it work on Edge?**  
> Yes, Edge is Chromium-based and should work with the same installation steps.

**Q: Will it work on Firefox?**  
> Not by default. Firefox would need extension compatibility changes.


<p align="center">
	Made for CUET Students
</p>
