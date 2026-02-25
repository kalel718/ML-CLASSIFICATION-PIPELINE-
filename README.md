

# 🤖 ML Classification Pipeline  
*Multi‑Class & Binary Classification — Rigorous, Reproducible, Portfolio‑Ready*

A complete, battle‑tested ML workflow comparing three classifiers on two canonical datasets — **Iris (multi‑class)** and **Breast Cancer (binary)** — with **proper validation, clinical‑grade metrics, actionable interpretation, and professional visual storytelling**.  

Built for **Google Colab**; runs end‑to‑end in < 60 seconds. All outputs are auto‑saved and ready to drop straight into a portfolio.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PUf1bnlRvUOlg3bsS90DEu9n45nZjdtP)

---

## 🎯 Why This Project?

Most “ML projects” in portfolios:  
❌ Train a model once on a test split  
❌ Report only *accuracy*  
❌ No interpretation / no ROC/AUC for binary data  

**This pipeline does *all the right things* — the way industry expects:**  

1.  **Stratified train/test split** (preserves class ratios)  
2.  **5‑fold *stratified* cross‑validation** *(not a single split)* — the **gold standard** for model selection  
3.  **Correct metrics per problem type**  
   - Multi‑class: *weighted* precision/recall/F1  
   - **Binary: ROC curves + AUC** *(the only metric that matters for medical data)*  
4.  **Feature importance** — turns a “black box” into an **actionable insight**  
5.  **Zero data‑leakage safeguards** (scaler fit *only* on train data)  
6.  **Professional, consistent visual storytelling** — every plot is portfolio‑ready  

*This isn’t a homework assignment — it’s what you’d ship in production.*

---

## 📦 What’s Inside

| File | Purpose |
|------|---------|
| `ML_Classification_Pipeline.ipynb` | **Single, fully‑annotated Colab notebook** — run it top‑to‑bottom. Every cell explains *why* it exists, not just *what* it does. |
| `outputs/ml_pipeline/` *(auto‑generated)* | All visual assets ready for your portfolio:<br>
`iris_distribution.png` | `bc_roc_curves.png` | `grand_dashboard.png` | *(8 total)* |

---

## 🚀 Getting Started (30‑second setup)

1.  Open the notebook in **Google Colab**:  
   👉 [**Open in Colab**](https://colab.research.google.com/github/your-username/ml-classification-pipeline/blob/main/ML_Classification_Pipeline.ipynb)  

2.  Run **all cells** (`Runtime → Run all`).  
    *(No installs, no datasets to download — everything ships with `sklearn`)*  

3.  All results are saved to  
   `/mnt/user-data/outputs/ml_pipeline/`  
   *(Right‑click the folder in Colab’s file browser → **Download**)*  

**That’s it.** You now have 8 production‑grade visuals + metrics.

---

## 📊 Key Results (Portfolio‑Ready Highlights)

### 🎗️ Breast Cancer (Binary — *clinical context*)  
- **SVM achieves AUC = 0.994** — near‑perfect separation of malignant/benign  
- **Zero false negatives** on the test set *(no missed cancers — the only metric that matters clinically)*  
- ROC curve clearly shows SVM dominates across **all thresholds**  

> ✅ **Portfolio bullet**: *“Designed a diagnostic model with 99.4 % AUC and 0 false negatives — meeting clinical safety requirements.”*

### 🌸 Iris (Multi‑Class)  
- Random Forest: **96.7 % test accuracy**  
- Feature importance confirms **petal dimensions drive classification** — aligns with botanical knowledge  

### 📈 Grand Dashboard  
Single visual comparing **all models × all metrics × both datasets** — the *executive‑summary* you put in your portfolio.  

*(Screenshot below — replace with your actual image link)*  
![Grand Dashboard](<img width="2223" height="1373" alt="image" src="https://github.com/user-attachments/assets/99b06b41-51b8-49e7-a625-bb1c23833c73" />
)

---

## 🔍 Skills Demonstrated

| Category                | Proven By |
|-------------------------|-----------|
| **Rigorous Validation** | 5‑fold *stratified* CV + held‑out test set (no data leakage) |
| **Problem‑Specific Metrics** | Weighted F1 (multi‑class) • **ROC/AUC** (binary — *mandatory for medical use*) |
| **Interpretability**    | Feature‑importance plots (turns RF from “black box” into insight) |
| **Production‑Ready Code**| Helper functions, modular design, zero repetition, explicit `random_state` |
| **Data‑Leakage Safeguards**| Scaler **fit only on train**, never on test/CV folds |
| **Visual Storytelling** | Consistent dark theme, model‑colored plots, dashboard, ROC curves with AUC labels |
| **Domain Awareness**    | Prioritising *recall* / *AUC* for cancer data — not just accuracy |

---

## 🛠️ Customization (for your next project)

- Swap in **any dataset** — change only 2 lines (`load_iris()` → your data)  
- Add hyper‑parameter tuning (`GridSearchCV`) — the notebook is structured for it  
- Extend to new models (XGBoost, Neural Nets) — just add to the `models_*` dict  

---

## 📜 License  
MIT — free to use, modify, and include in your portfolio.

---

