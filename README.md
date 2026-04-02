# 🏀 NBA Award Voting Share Prediction

## 📌 Project Overview
This project builds a machine learning model to predict **NBA award voting share** using player performance metrics.

The goal is to understand how well **advanced analytics explain real-world voting outcomes** and to frame award voting as a **predictive ranking problem**.

This project follows an end-to-end workflow:
- Data exploration  
- Feature engineering  
- Model development  
- Evaluation and interpretation  

---

## 🎯 Problem Framing
NBA awards (MVP / All-NBA) are influenced by:
- Player performance  
- Advanced metrics  
- Team success  
- Narrative factors  

This project focuses on the measurable component:

**Given a player’s season stats, can we predict their share of award votes?**

---

## 📊 Dataset
- ~12,700 player-season records  
- Each row represents one player in one season  

### Target
- `points_share` → proportion of total votes received  

### Features
- Traditional stats (PTS, AST, REB)  
- Advanced metrics (PER, BPM, VORP)  
- Efficiency metrics  
- Team-related indicators  

---

## 🔍 Exploratory Analysis

Key analysis steps:
- Distribution of vote share  
- Correlation between metrics and voting outcomes  
- Multicollinearity checks  
- Comparison of elite vs average players  

### Key Findings
- Vote share is **heavily skewed** (most players receive zero votes)  
- A small group of elite players captures the majority of votes  
- **PER, VORP, and BPM show strong relationships with vote share**  
- Clear statistical separation between award-level players and the rest of the league  

---

## 🛠️ Feature Engineering

Steps taken:
- Removed redundant / low-signal features  
- Selected high-impact advanced metrics  
- Cleaned and standardized numeric inputs  
- Prepared a model-ready dataset  

Focus was placed on interpretability and predictive strength.

---

## 🤖 Modeling

### Models Tested
- Linear Regression (baseline)  
- Regularized regression  
- Tree-based regression models  

### Evaluation
- Train/test split  
- Metrics:
  - R²  
  - RMSE  

---

## 📈 Results

- Advanced metrics explain a meaningful portion of vote share variance  
- **PER and VORP consistently rank as top predictors**  
- Linear models capture overall trends but struggle with MVP-level outliers  

### Interpretation
Voting outcomes align closely with performance metrics, but are not fully explained by them due to narrative and contextual factors.

---

## 💡 Key Takeaways

- Award voting can be modeled as a **data-driven ranking problem**  
- Advanced metrics are strong proxies for voter behavior  
- Non-quantifiable factors limit predictive accuracy  

---

## 🚀 Future Improvements
- Reframe as classification (vote vs no vote)  
- Add team-level features  
- Incorporate narrative/time-based signals  
- Use ensemble models  
- Compare predicted vs actual rankings  

---

## 🧰 Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Jupyter  

---

## 📁 Repository Structure
- 01_all_nba_vote_share_exploratory_analysis.ipynb  
- 02_all_nba_vote_share_preprocessing.ipynb  
- 03_all_nba_vote_share_modeling.ipynb  

---

## 📌 Portfolio Context

This project demonstrates:
- End-to-end ML workflow ownership  
- Strong feature engineering  
- Applied regression modeling  
- Model interpretation  

**Transferable to:**
- Customer scoring  
- Marketing analytics  
- Ranking systems  
- Decision-support modeling  
