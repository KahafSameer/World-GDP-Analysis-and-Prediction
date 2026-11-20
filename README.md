<div align="center">

# 🌍 World GDP — Analysis & Prediction

**A Streamlit dashboard + ML predictor for exploring and estimating GDP per capita around the world.**

<img src="https://sl.bing.net/fhdNHclIs8q" alt="World GDP Analysis banner" width="100%"/>

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-App-ff4b4b)](https://streamlit.io/)
[![pandas](https://img.shields.io/badge/pandas-Data%20Wrangling-150458)](https://pandas.pydata.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-ff9f1c)](https://scikit-learn.org/stable/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#-contributing)

</div>

> **Tip:** Add your own images/GIFs in the `assets/` folder using the filenames referenced below to make the README look perfect ✨.

---

## 📌 Table of Contents

* [Overview](#-overview)
* [Features](#-features)
* [Demo](#-demo)
* [Quick Start](#-quick-start)
* [How to Use](#-how-to-use)
* [Data & Columns](#-data--columns)
* [Analysis Highlights](#-analysis-highlights)
* [Top 5 by Region](#-top-5-by-region)
* [Tech Stack](#-tech-stack)
* [Project Structure](#-project-structure)
* [Roadmap](#-roadmap)
* [Contributing](#-contributing)
* [License](#-license)

---

## 🔎 Overview

This repository provides a clean, interactive **Streamlit** dashboard for global **GDP per capita** exploration, plus a simple **predictive system** that estimates a country's GDP per capita based on selected features. Upload your CSV, explore trends, and generate predictions in seconds.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/overview_dark.png">
  <img src="assets/overview_light.png" alt="App overview screenshot" width="100%"/>
</picture>

---

## ✨ Features

* 📈 **Interactive dashboard** with filters, summaries, and charts
* 🤖 **Predictive model** (scikit‑learn regressor) for GDP per capita
* 🧹 **Data preprocessing** (missing values, type casting, feature selection)
* 📊 **Top 15 countries by GDP per capita** visualization
* 🌎 **Top 5 countries per region** view for quick comparisons
* 💾 **Local CSV upload** — bring your own dataset

---

## 🎬 Demo

Add a short screen capture of your app to make this pop:

```text
assets/demo.gif   ← put a GIF here (3–8 seconds is perfect)
```

```html
<p align="center">
  <img src="assets/demo.gif" alt="World GDP demo" width="85%"/>
</p>
```

---

## 🚀 Quick Start

```bash
# 1) Clone the repo
git clone https://github.com/KahafSameer/World-GDP-Analysis-and-Prediction.git
cd World-GDP-Analysis-and-Prediction

# 2) Create & activate a virtual environment (optional but recommended)
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate

# 3) Install dependencies
pip install -r requirements.txt

# 4) Launch the Streamlit app
streamlit run app.py
```

> Then open the local URL Streamlit prints (usually `http://localhost:8501`).

---

## 🧭 How to Use

1. **Upload CSV** with GDP and country data.
2. Explore **summary stats**, **regional breakdowns**, and **visualizations**.
3. Use the **Predict** panel to input features and get an estimated **GDP per capita**.
4. Dive into **Top 15** and **Top 5 by Region** charts for quick insights.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/dashboard_dark.png">
  <img src="assets/dashboard_light.png" alt="Dashboard screenshot" width="100%"/>
</picture>

---

## 🧾 Data & Columns

The app expects a CSV with (at minimum) columns similar to:

```csv
Country,Region,GDP_per_capita,Literacy_rate,Agriculture,Year
Norway,Europe,75420,99.0,1.7,2022
Pakistan,Asia,1500,58.0,23.1,2022
```

* **GDP\_per\_capita**: numeric
* **Literacy\_rate**: numeric (%)
* **Agriculture**: numeric (%) or index
* **Region**: categorical (e.g., Europe, Asia)
* **Year**: optional but recommended

> Your actual column names can be mapped/renamed in the preprocessing step of the app if implemented.

---

## 🔬 Analysis Highlights

* Computes **average GDP**, **literacy**, and **agriculture** per region
* Visualizes **Top 15 countries** by GDP per capita
* Shows trend snapshots and distribution plots

<p align="center">
  <img src="assets/charts_top15.png" alt="Top 15 GDP per capita chart" width="85%"/>
</p>

---

## 🥇 Top 5 by Region

Quickly compare regional leaders with a single chart.

<p align="center">
  <img src="assets/charts_top5_region.png" alt="Top 5 per region chart" width="85%"/>
</p>

---

## 🧰 Tech Stack

* **Python** — data and ML
* **Streamlit** — interactive UI
* **pandas / numpy** — data wrangling
* **matplotlib / seaborn** — plots
* **scikit‑learn** — prediction model

---

## 📁 Project Structure

```
world-gdp-analysis/
├─ app.py
├─ requirements.txt
├─ README.md
├─ data/                 # optional local data samples
├─ models/               # saved models (if any)
├─ utils/                # helper modules (preprocessing, viz, etc.)
├─ assets/               # images used in README/app (add your own)
│  ├─ banner.png
│  ├─ overview_light.png
│  ├─ overview_dark.png
│  ├─ dashboard_light.png
│  ├─ dashboard_dark.png
│  ├─ demo.gif
│  ├─ charts_top15.png
│  └─ charts_top5_region.png
└─ LICENSE
```

---

## 🗺️ Roadmap

* [ ] Add example dataset in `data/`
* [ ] Export predictions as CSV
* [ ] Add more model options (e.g., RandomForest, XGBoost)
* [ ] Country-level time series trends
* [ ] Deployment guide (Streamlit Cloud / Docker)

---

## 🤝 Contributing

Contributions are welcome! To propose changes:

1. **Fork** the repo
2. **Create a branch**: `git checkout -b feat/awesome-thing`
3. **Commit**: `git commit -m "feat: add awesome thing"`
4. **Push**: `git push origin feat/awesome-thing`
5. **Open a PR** and describe your changes

---

## 📜 License

This project is licensed under the **MIT License**. See [`LICENSE`](LICENSE) for details.

---

<div align="center">

Made with ❤️ for data explorers everywhere.

</div>
