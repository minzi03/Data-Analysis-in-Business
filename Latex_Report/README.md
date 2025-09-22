# 📄 LaTeX Report Documentation

The **`Latex_Report/`** directory contains the final research paper and supporting files written in **LaTeX (IEEE style)**. This report consolidates all analyses, models, results, and discussions from the project *Forecasting Stock Price Accuracy for Vietnamese Pharmaceutical Firms*.

---

## 📂 Structure Overview

```

Latex\_Report/
├── Report.tex                # Main LaTeX source file (IEEE format)
├── ieeeojies.cls             # IEEE journal class file
└── bibliography/             # Bibliographic references
├── README
├── IEEEabrv.bib
├── IEEEexample.bib
├── IEEEfull.bib
└── mybibfile.bib

```

---

## 📘 File Descriptions

### 🔹 `Report.tex`
- The main LaTeX document of the project.
- Written in **IEEE OJIES** style.
- Includes:
  - Title, author information, and affiliations.
  - Abstract and keywords.
  - Sections: **Introduction, Related Works, Materials, Methodology, Results, Acknowledgment, References**.
  - Tables and figures describing descriptive statistics, regression plots, and forecasting results.

### 🔹 `ieeeojies.cls`
- Class file that defines formatting rules following the **IEEE Open Journal of the Industrial Electronics Society** style.
- Ensures correct margins, fonts, title formatting, and bibliography style.

### 🔹 `bibliography/`
Contains reference libraries in BibTeX format:
- **`IEEEabrv.bib`** – Standard IEEE journal abbreviations.
- **`IEEEexample.bib`** – Example references for formatting guidance.
- **`IEEEfull.bib`** – Full IEEE bibliographic entries.
- **`mybibfile.bib`** – Project-specific references (related works, datasets, algorithms, etc.).
- **`README`** – Instructions for managing BibTeX citations.

---

## 🛠 Usage Instructions

1. Open `Report.tex` in a LaTeX editor (Overleaf, TeXstudio, VS Code with LaTeX Workshop).
2. Compile with **PDFLaTeX** or **XeLaTeX** (preferred for UTF-8 and figures).
3. Bibliography is automatically generated using BibTeX files from `/bibliography/`.
4. Figures are included from the `bibliography/Figure/` path.

---

## 📑 Report Content Highlights

- **Datasets:** Historical daily stock data (2019–2024) from Investing.com for three pharmaceutical firms (*DHT, DP3, AMV*).  
- **Models:** Statistical (LR, ARIMA, FFT), ML (LightGBM, LR-CF-DP), DL (RNN, GRU, LSTM).  
- **Results:** Performance comparison using RMSE, MAPE, MSLE across 30-, 60-, and 90-day horizons.  
- **Findings:** LSTM achieved **MAPE < 3.5%**, outperforming classical models (ARIMA ≥ 30%, FFT ≥ 60%).  
- **Applications:** Investment decision support, risk management, and portfolio optimization.  

---

## 🎯 Learning Outcomes

- Practice writing a **scientific paper in IEEE format**.  
- Gain experience in **organizing references with BibTeX**.  
- Present results with **professional tables and figures**.  
- Prepare project documentation suitable for publication or academic submission.  
