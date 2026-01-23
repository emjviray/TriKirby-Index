# TriKirby Index

A percentile-based pitching command statistic inspired by the **Kirby Index** (Michael Rosen, FanGraphs), expanded into the **TriKirby Index** to quantify the command and effectiveness of each **UC San Diego (UCSD) Tritons pitcher’s pitch types** heading into the 2026 season.

---

## Overview

The **TriKirby Index** is a methodology-driven evaluation framework designed to measure pitcher command across pitch types using percentile-based standardized deviations. This project applies a data-science pipeline to transform pitch-level tracking data into interpretable pitcher scores that reflect both **mechanical consistency** and **command quality**.

This work was created as a pitching evaluation tool and presented in a way that can support:
- player development & coaching decisions  
- injury prevention insights  
- pitcher comparisons across NCAA D1  
- pitch-type specific command grading  

---

## Key Ideas

This project expands on the Kirby Index concept by building a composite score using **four primary pitch-command components**:

- **Vertical Release Angle**
- **Horizontal Release Angle**
- **Vertical Release Location**
- **Horizontal Release Location**

Each component is standardized using **percentile-based deviations**, allowing pitchers to be evaluated relative to distribution-based baselines.

---

## Methods Used

### 1. Data Preparation
- Pitch-by-pitch data cleaning, filtering, and formatting  
- Pitch type grouping and minimum pitch thresholds  
- Per-pitch and per-player aggregation  

### 2. Percentile-Based Standardization
Each command-related feature is converted into standardized deviation values based on distribution percentiles.

### 3. Feature Weighting
Two machine learning approaches are applied to compute feature weights and importance:
- **Logistic Regression** (linear weights for interpretability)
- **Random Forests** (feature importance extraction)

### 4. Final Score Generation
- Component deviations are weighted and combined into a composite **TriKirby Score**
- Scores can be broken down by:
  - pitch type
  - pitcher
  - team
  - season averages (NCAA baselines)

---

## Outputs

This repo includes:
- Jupyter notebooks with full pipeline implementation
- A finalized report exported as PDF
- Spreadsheet-compatible outputs for ranking and comparisons

Main results allow you to:
- rank pitchers by pitch-type command
- compare team command distributions
- identify strengths/weaknesses by pitch arsenal

---

## Tech Stack / Tools

- **Python**
- **Jupyter Notebook**
- **Pandas / NumPy**
- **Matplotlib / Seaborn**
- **Scikit-learn**
  - Logistic Regression
  - Random Forests
  - PCA (where applicable)

---

## Repository Contents

| File | Description |
|------|------------|
| `TriKirby Index Final Sheet.pdf` | Final PDF report / exported sheet output |
| `TriKirbyIndex (8).ipynb` | Main TriKirby notebook pipeline |
| `TriKirbyIndexNCAA.ipynb` | NCAA-wide baseline calculations / comparisons |
| `README.md` | Project overview and documentation |

---

## Inspiration / Reference

This project is inspired by the Kirby Index created by Michael Rosen on FanGraphs:  
https://blogs.fangraphs.com/introducing-the-kirby-index-a-new-way-to-quantify-command/

---

## Author

**Emmanuel Viray III**  
Data Analyst – UCSD Baseball | Cognitive Science (Machine Learning & Neural Computation) @ UC San Diego  

If you’re interested in baseball analytics, machine learning, or sports research — feel free to connect!

---
